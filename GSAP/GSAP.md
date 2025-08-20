GSAP -> An animation library.

GSAP stands for GreenSock Animation Platform. It is a JavaScript library used for creating high-performance animations on the web. GSAP is known for its speed, flexibility, and ease of use, allowing developers to animate various HTML elements, CSS properties, SVG graphics, and more. 

gsap.to("#id",{
    x: 1200,
    duration: 2,
    delay: 1,
    rotate: 360,
    repeat: -1,
    yoyo: true
})

gsap.from("#id",{
    x: 1200,
    duration: 2,
    delay: 1,
    rotate: 360,
    repeat: -1,
    yoyo: true
})


repeat: 1       // run the animation + 1 time more
repeat: -1      // run the animation in infinite
yoyo: true      // it bounce back the animation from the final position to initial position