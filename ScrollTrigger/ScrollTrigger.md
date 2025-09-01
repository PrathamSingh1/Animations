ScrollTrigger ->

use the gsap cdn above the script tag

order ->
    GSAP
    SCROLL TRIGGER
    JAVASCRIPT

->> when the element start hit the page scroller-start the animation will be start.




Example 1 ->

gsap.from("#page1 #box", {
    scale: 0,
    delay: 1,
    duration: 2,
    rotate: 360
})

gsap.from("#page2 #box", {
    scale: 0,
    duration: 2,
    rotate: 360,
    scrollTrigger: {
        trigger: "#page2 #box",
        scroller: "body",
        markers: true,
        start: "top 60%"
    }
})




Example 2 ->



gsap.from("#page2 h1", {
    opacity: 0,
    x: 500,
    duration: 2,
    scrollTrigger: {
        trigger: "#page2 h1",
        scroller: "body",
        markers: true,
        start: "top 50%"
    }
})

gsap.from("#page2 h2", {
    opacity: 0,
    x: -500,
    duration: 2,
    scrollTrigger: {
        trigger: "#page2 h2",
        scroller: "body",
        markers: true,
        start: "top 50%"
    }
})