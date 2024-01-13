<script>
import gsap from 'gsap';



export default {
  methods: {
    // where the animation will start from
    beforeEnter(el) {
      el.style.opacity = '0'
      
    },
    // where the animation will end up
    enter(el) {
      gsap.to(el, {
        duration: 3,
        y: 0,
        opacity: 1,
        repeat: -1,
        ease:'power1.inOut',
        yoyo: true
      })
    },
    beforeCircle(el){
        
    const elementWidth = el.clientWidth;

    const viewportWidth = window.innerWidth;

    const initialY = (viewportWidth - elementWidth) / 2;

    const initialX = -initialY;
        gsap.from(el ,{
            x: initialX,
            duration:1,
        })
    },  
    circle(el){
        gsap.to(el ,{
            x: 0,
            opacity:1,
            duration: 2,
            ease:'power1.inOut'
        })
    },
    beforeMoon(el){
        
        const elementWidth = el.clientWidth;
    
        const viewportWidth = window.innerWidth;
    
        const initialY = (viewportWidth - elementWidth) / 2;
    
        const initialX = -initialY;
            gsap.from(el ,{
                x: -initialY,
                duration:1,
            })
        },  
        moon(el){
            gsap.to(el ,{
                x: 0,
                opacity:1,
                duration: 2,
                ease:'power1.inOut'
            })
        },

  }
}




</script>

<template>
    <svg viewBox="0 0 1920 1080" fill="none"  style="width: max-content;height: max-content; z-index: -1;" class="fixed top-0">
        <g clip-path="url(#clip0_11_2)">
            <rect width="1920" height="1080" fill="#216583"/>
            <rect width="1920" height="1080" fill="black" fill-opacity="0.2"/>
            <g filter="url(#filter0_f_11_2)">
                <rect x="-406" y="997" width="2510" height="200" fill="#F76262"/>
            </g>
            <transition
                appear
                @before-enter="beforeEnter"
                @enter="enter"
            >
                <g id="shadow" filter="url(#filter1_f_11_2)">
                    <ellipse cx="1693.5" cy="530" rx="240.5" ry="234" fill="white"/>
                </g>
            </transition>
            
            <transition
                appear
                @before-enter="before"
                @enter="circle"
            >
            <g class="myCircle absolute" filter="url(#filter2_b_11_2)">
                <ellipse cx="1680" cy="530.5" rx="227" ry="223.5" fill="black"/>
            </g>
            </transition>
            <line class="lines" x1="120" y1="474" x2="1764" y2="474" stroke="white" stroke-width="10"/>
            <line class="lines" x1="120" y1="584" x2="1764" y2="584" stroke="white" stroke-width="10"/>
            <line class="lines" x1="120" y1="531" x2="1764" y2="531" stroke="white" stroke-width="10"/>
            <g filter="url(#filter3_f_11_2)">
                <line x1="42" y1="440" x2="1833" y2="440" stroke="white" stroke-width="10"/>
            </g>
            <g filter="url(#filter4_f_11_2)">
                <line x1="42" y1="626" x2="1833" y2="626" stroke="white" stroke-width="10"/>
            </g>
            <g filter="url(#filter5_f_11_2)">
                <line x1="42" y1="537" x2="1833" y2="537" stroke="white" stroke-width="10"/>
            </g>
            <g class="myShadows" filter="url(#filter6_f_11_2)">
                <path d="M225.168 345.326L315 366.105L262.208 320.391L211.119 307H176.208L119.584 320.391L72.3267 345.326L47.6337 406.278L31.4554 440.448L14 512.945V596.985L31.4554 685.181L57.8515 742.439L107.238 776.609L211.119 790L315 765.065V727.201L272.851 742.439H211.119L137.465 702.266L72.3267 612.685L57.8515 512.945L93.1881 427.057L137.465 377.649L225.168 345.326Z" fill="white"/>
            </g>
            <Transition appear
                @before-enter="beforeMoon"
                @enter="moon" >
                <rect id="moon" width="543.377" height="520.396" transform="matrix(-0.808468 -0.588541 -0.588541 0.808468 597.577 473.799)" fill="url(#pattern0)"/>
            </Transition>    
            </g>
            <defs>
    <filter id="filter0_f_11_2" x="-760.9" y="642.1" width="3219.8" height="909.8" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
        <feFlood flood-opacity="0" result="BackgroundImageFix"/>
        <feBlend mode="normal" in="SourceGraphic" in2="BackgroundImageFix" result="shape"/>
        <feGaussianBlur stdDeviation="177.45" result="effect1_foregroundBlur_11_2"/>
    </filter>
    <filter id="filter1_f_11_2" x="1053" y="-104" width="1281" height="1268" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
        <feFlood flood-opacity="0" result="BackgroundImageFix"/>
        <feBlend mode="normal" in="SourceGraphic" in2="BackgroundImageFix" result="shape"/>
        <feGaussianBlur stdDeviation="200" result="effect1_foregroundBlur_11_2"/>
    </filter>
    <filter id="filter2_b_11_2" x="1449" y="303" width="462" height="455" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
        <feFlood flood-opacity="0" result="BackgroundImageFix"/>
        <feGaussianBlur in="BackgroundImageFix" stdDeviation="2"/>
        <feComposite in2="SourceAlpha" operator="in" result="effect1_backgroundBlur_11_2"/>
        <feBlend mode="normal" in="SourceGraphic" in2="effect1_backgroundBlur_11_2" result="shape"/>
    </filter>
    <filter id="filter3_f_11_2" x="-108" y="285" width="2091" height="310" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
    <feFlood flood-opacity="0" result="BackgroundImageFix"/>
    <feBlend mode="normal" in="SourceGraphic" in2="BackgroundImageFix" result="shape"/>
    <feGaussianBlur stdDeviation="75" result="effect1_foregroundBlur_11_2"/>
    </filter>
    <filter id="filter4_f_11_2" x="-108" y="471" width="2091" height="310" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
    <feFlood flood-opacity="0" result="BackgroundImageFix"/>
    <feBlend mode="normal" in="SourceGraphic" in2="BackgroundImageFix" result="shape"/>
    <feGaussianBlur stdDeviation="75" result="effect1_foregroundBlur_11_2"/>
    </filter>
    <filter id="filter5_f_11_2" x="-108" y="382" width="2091" height="310" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
    <feFlood flood-opacity="0" result="BackgroundImageFix"/>
    <feBlend mode="normal" in="SourceGraphic" in2="BackgroundImageFix" result="shape"/>
    <feGaussianBlur stdDeviation="75" result="effect1_foregroundBlur_11_2"/>
    </filter>
    <filter id="filter6_f_11_2" x="-153" y="140" width="635" height="817" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
    <feFlood flood-opacity="0" result="BackgroundImageFix"/>
    <feBlend mode="normal" in="SourceGraphic" in2="BackgroundImageFix" result="shape"/>
    <feGaussianBlur stdDeviation="83.5" result="effect1_foregroundBlur_11_2"/>
    </filter>
    <pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1">
    <use xlink:href="#image0_11_2" transform="matrix(0.003125 0 0 0.003263 0 -0.0220797)"/>
    </pattern>
    <clipPath id="clip0_11_2">
    <rect width="1920" height="1080" fill="white"/>
    </clipPath>
    <image id="image0_11_2" width="320" height="320" xlink:href="data:image/png;base64,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"/>
    </defs>
    </svg>
    
</template>