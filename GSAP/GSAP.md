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




GSAP Timeline and how to control it ->


var tl = gsap.timeline()

tl.to("#box1", {
    x: 1500,
    rotate: 360,
    duration: 1.5,
    delay: 1
})

tl.to("#box2", {
    x: 1500,
    duration: 1.5
})


Example code 2 ->

var tl = gsap.timeline()

tl.from("h2", {
    y: -30,
    opacity: 0,
    duration: 1,
    delay: 0.5
})

tl.from("h4", {
    y: -30,
    opacity: 0,
    duration: 1,
    stagger: 0.3
})

tl.from("h1", {
    y: 20,
    opacity: 0,
    duration: 0.5,
    scale: 0.2
})