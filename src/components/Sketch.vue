<template>
  <div id="sketch">

  </div>
</template>

<script>

export default {
    components: {},
    props: [],
    data() {
        return {

        }
    },
    mounted() {
        const sketch = function(p5) {
            let deltaX;
            let deltaY;
            p5.setup = () => {
                p5.createCanvas(p5.windowWidth, p5.windowHeight, p5.WEBGL);
                deltaX = 0;
                deltaY = 0;

                // p5.noCursor();
            }

            p5.draw = () => {

                p5.background(255);
                
                deltaX = p5.lerp(deltaX, p5.mouseX, .1);
                deltaY = p5.lerp(deltaY, p5.mouseY, .1);

               
                p5.push();
                p5.translate(deltaX, deltaY,0);
                p5.noStroke();
                p5.fill(0,0,255);
                p5.ellipse(-p5.width/2, -p5.height/2, 400,400);
                p5.pop();
            }

            p5.windowResized = () => {
                p5.resizeCanvas(p5.windowWidth, p5.windowHeight);
            }
        }

        const P5 = require('p5');
        new P5(sketch, "sketch");
    }
}
</script>

<style>
    #sketch {
        width: 100%;
        height: 100%;
        position: fixed;
        top: 0;
        left: 0;
        z-index: 0;
        filter: blur(100px);
    }

    canvas {
        z-index: 0;
        
    }
</style>