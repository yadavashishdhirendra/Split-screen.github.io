# VanillaJS_DoubleVerticlSlider

View Project here: https://timmanas.github.io/VanillaJS_DoubleVerticlSlider

**Tips & Tricks:**

1. The slider is actually just a transform css property which moves the left or right side up or down

2. There are two things which get translated ...left and Right slider containerrs.
   One moves in +Y direction, other in -Y direction

Ex:
slideRight.style.transform = translateY(-${ activeSlideIndex \* sliderHeight }px)

slideLeft.style.transform = translateY(${activeSlideIndex \* sliderHeight}px)∂

3. The reason image stay in place is due to the
   .slider-container {
   position: relative;
   overflow: hidden;
   width: 100vw;
   height: 100vh;
   }

4. Removing the transform property, will simply make the image appear instead of any transition
   Ex:
   transition: transform 3.5s ease-in-out;
