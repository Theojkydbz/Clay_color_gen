<template>
    <div class="like">
        <transition name="fade" appear mode="out-in">

            <svg v-if="visible" key="visible" width="40vh" height="30vh" viewBox="0 0 523 304" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                <defs>
                    
                    <path @click="Toggle" v-bind:href="[coloring]" d="M113.2249,40 L409.7751,40 C433.846106,40 442.574834,42.5062915 451.374834,47.212583 C460.174834,51.9188745 467.081125,58.825166 471.787417,67.625166 C476.493708,76.425166 479,85.1538944 479,109.2249 L479,186.7751 C479,210.846106 476.493708,219.574834 471.787417,228.374834 C467.081125,237.174834 460.174834,244.081125 451.374834,248.787417 C442.574834,253.493708 433.846106,256 409.7751,256 L113.2249,256 C89.1538944,256 80.425166,253.493708 71.625166,248.787417 C62.825166,244.081125 55.9188745,237.174834 51.212583,228.374834 C46.5062915,219.574834 44,210.846106 44,186.7751 L44,109.2249 C44,85.1538944 46.5062915,76.425166 51.212583,67.625166 C55.9188745,58.825166 62.825166,51.9188745 71.625166,47.212583 C80.425166,42.5062915 89.1538944,40 113.2249,40 Z" id="path-1"></path>
                    <filter x="-15.6%" y="-29.6%" width="131.3%" height="163.0%" filterUnits="objectBoundingBox" id="filter-2">
                        <feOffset dx="0" dy="4" in="SourceAlpha" result="shadowOffsetOuter1"></feOffset>
                        <feGaussianBlur stdDeviation="22" in="shadowOffsetOuter1" result="shadowBlurOuter1"></feGaussianBlur>
                        <feColorMatrix values="0 0 0 0 0   0 0 0 0 0   0 0 0 0 0  0 0 0 0.264605978 0" type="matrix" in="shadowBlurOuter1"></feColorMatrix>
                    </filter>
                    <filter x="-12.6%" y="-23.6%" width="125.3%" height="150.9%" filterUnits="objectBoundingBox" id="filter-3">
                        <feGaussianBlur stdDeviation="11" in="SourceAlpha" result="shadowBlurInner1"></feGaussianBlur>
                        <feOffset dx="0" dy="0" in="shadowBlurInner1" result="shadowOffsetInner1"></feOffset>
                        <feComposite in="shadowOffsetInner1" in2="SourceAlpha" operator="arithmetic" k2="-1" k3="1" result="shadowInnerInner1"></feComposite>
                        <feColorMatrix values="0 0 0 0 0   0 0 0 0 0   0 0 0 0 0  0 0 0 0.194774683 0" type="matrix" in="shadowInnerInner1" result="shadowMatrixInner1"></feColorMatrix>
                        <feGaussianBlur stdDeviation="2" in="SourceAlpha" result="shadowBlurInner2"></feGaussianBlur>
                        <feOffset dx="0" dy="0" in="shadowBlurInner2" result="shadowOffsetInner2"></feOffset>
                        <feComposite in="shadowOffsetInner2" in2="SourceAlpha" operator="arithmetic" k2="-1" k3="1" result="shadowInnerInner2"></feComposite>
                        <feColorMatrix values="0 0 0 0 0   0 0 0 0 0   0 0 0 0 0  0 0 0 0.184612772 0" type="matrix" in="shadowInnerInner2" result="shadowMatrixInner2"></feColorMatrix>
                        <feMerge>
                            <feMergeNode in="shadowMatrixInner1"></feMergeNode>
                            <feMergeNode in="shadowMatrixInner2"></feMergeNode>
                        </feMerge>
                    </filter>
                      
                </defs>
                <g id="Page-1" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                    <g id="iphone">
                        <use fill="black" fill-opacity="1" filter="url(#filter-2)" xlink:href="#path-1"></use>
                        <use :fill="[coloring]" fill-rule="evenodd" xlink:href="#path-1"></use>
                        <use fill="black" fill-opacity="1" filter="url(#filter-3)" xlink:href="#path-1"></use>
                    </g>
                </g>
            </svg>


            <svg v-else key="invisible" width="40vh" height="30vh" viewBox="0 0 523 304" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                <defs>
                    <path @click="Toggle" d="M113.2249,40 L409.7751,40 C433.846106,40 442.574834,42.5062915 451.374834,47.212583 C460.174834,51.9188745 467.081125,58.825166 471.787417,67.625166 C476.493708,76.425166 479,85.1538944 479,109.2249 L479,186.7751 C479,210.846106 476.493708,219.574834 471.787417,228.374834 C467.081125,237.174834 460.174834,244.081125 451.374834,248.787417 C442.574834,253.493708 433.846106,256 409.7751,256 L113.2249,256 C89.1538944,256 80.425166,253.493708 71.625166,248.787417 C62.825166,244.081125 55.9188745,237.174834 51.212583,228.374834 C46.5062915,219.574834 44,210.846106 44,186.7751 L44,109.2249 C44,85.1538944 46.5062915,76.425166 51.212583,67.625166 C55.9188745,58.825166 62.825166,51.9188745 71.625166,47.212583 C80.425166,42.5062915 89.1538944,40 113.2249,40 Z" id="path-1"></path>
                    <filter x="-15.6%" y="-29.6%" width="131.3%" height="163.0%" filterUnits="objectBoundingBox" id="filter-2">
                        <feOffset dx="0" dy="4" in="SourceAlpha" result="shadowOffsetOuter1"></feOffset>
                        <feGaussianBlur stdDeviation="22" in="shadowOffsetOuter1" result="shadowBlurOuter1"></feGaussianBlur>
                        <feColorMatrix values="0 0 0 0 0   0 0 0 0 0   0 0 0 0 0  0 0 0 0.264605978 0" type="matrix" in="shadowBlurOuter1"></feColorMatrix>
                    </filter>
                    <filter x="-12.6%" y="-23.6%" width="125.3%" height="150.9%" filterUnits="objectBoundingBox" id="filter-3">
                        <feGaussianBlur stdDeviation="11" in="SourceAlpha" result="shadowBlurInner1"></feGaussianBlur>
                        <feOffset dx="0" dy="0" in="shadowBlurInner1" result="shadowOffsetInner1"></feOffset>
                        <feComposite in="shadowOffsetInner1" in2="SourceAlpha" operator="arithmetic" k2="-1" k3="1" result="shadowInnerInner1"></feComposite>
                        <feColorMatrix values="0 0 0 0 0   0 0 0 0 0   0 0 0 0 0  0 0 0 0.194774683 0" type="matrix" in="shadowInnerInner1" result="shadowMatrixInner1"></feColorMatrix>
                        <feGaussianBlur stdDeviation="2" in="SourceAlpha" result="shadowBlurInner2"></feGaussianBlur>
                        <feOffset dx="0" dy="0" in="shadowBlurInner2" result="shadowOffsetInner2"></feOffset>
                        <feComposite in="shadowOffsetInner2" in2="SourceAlpha" operator="arithmetic" k2="-1" k3="1" result="shadowInnerInner2"></feComposite>
                        <feColorMatrix values="0 0 0 0 0   0 0 0 0 0   0 0 0 0 0  0 0 0 0.184612772 0" type="matrix" in="shadowInnerInner2" result="shadowMatrixInner2"></feColorMatrix>
                        <feMerge>
                            <feMergeNode in="shadowMatrixInner1"></feMergeNode>
                            <feMergeNode in="shadowMatrixInner2"></feMergeNode>
                        </feMerge>
                    </filter>
                </defs>
                <g id="Page-1" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                    <g id="iphone-copy">
                        <use fill="black" fill-opacity="1" filter="url(#filter-2)" xlink:href="#path-1"></use>
                        <use :fill="[coloring]" fill-rule="evenodd" xlink:href="#path-1"></use>
                        <use fill="black" fill-opacity="1" filter="url(#filter-3)" xlink:href="#path-1"></use>
                    </g>
                </g>
            </svg>

        </transition>

        <transition name="select" appear mode="out-in">

        <svg v-if="visible1" width="35px" height="38px" viewBox="0 0 50 43" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
            <g id="Page-1" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd" fill-opacity="0">
                <g id="heart" transform="translate(2.000000, 2.000000)" fill="#000000" fill-rule="nonzero" stroke="#747D8C" stroke-width="4">
                    <path @click="yesToggle" d="M42.227509,3.1236 C37.7564679,-1.0412 30.507808,-1.0412 26.0362321,3.1236 L23.0002674,5.95134286 L19.963233,3.1236 C15.4927268,-1.0412 8.24406693,-1.0412 3.77249102,3.1236 C-1.25749701,7.80845714 -1.25749701,15.4052 3.77249102,20.0900571 L23.0002674,38 L42.227509,20.0900571 C47.257497,15.4046571 47.257497,7.80845714 42.227509,3.1236 Z" id="Shape"></path>
                </g>
            </g>
        </svg>

        <svg v-else key="invisible1" width="35px" height="38px" viewBox="0 0 50 43" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
            <g id="Page-1" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                <g id="heart" transform="translate(2.000000, 2.000000)" fill="#747D8C" fill-rule="nonzero" stroke="#747D8C" stroke-width="4">
                    <path  @click="noToggle" d="M42.227509,3.1236 C37.7564679,-1.0412 30.507808,-1.0412 26.0362321,3.1236 L23.0002674,5.95134286 L19.963233,3.1236 C15.4927268,-1.0412 8.24406693,-1.0412 3.77249102,3.1236 C-1.25749701,7.80845714 -1.25749701,15.4052 3.77249102,20.0900571 L23.0002674,38 L42.227509,20.0900571 C47.257497,15.4046571 47.257497,7.80845714 42.227509,3.1236 Z" id="Shape"></path>
                </g>
            </g>
        </svg>

        </transition>
        
        <p>MADE WITH <img src="../assets/logo.png" alt="" style="width:3vh; transform:translateY(1vh)"> BY <a href="http://www.theogeiller.com">THEO GEILLER</a></p>
  
        <svg width="52px" height="18px" viewBox="0 0 52 18" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
            <g id="Page-1" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd" stroke-linecap="round" stroke-linejoin="round">
             <polyline id="Path-6" stroke="#747D8C" stroke-width="6" points="3 3 25.6544694 14.7620376 49 3"></polyline>
            </g>
        </svg>
            <ul>

                <li class="like" v-for="like in likes">

                    <svg width="40vh" height="30vh" viewBox="0 0 523 304" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                                    <defs>
                                        <path @click="copyClip" d="M113.2249,40 L409.7751,40 C433.846106,40 442.574834,42.5062915 451.374834,47.212583 C460.174834,51.9188745 467.081125,58.825166 471.787417,67.625166 C476.493708,76.425166 479,85.1538944 479,109.2249 L479,186.7751 C479,210.846106 476.493708,219.574834 471.787417,228.374834 C467.081125,237.174834 460.174834,244.081125 451.374834,248.787417 C442.574834,253.493708 433.846106,256 409.7751,256 L113.2249,256 C89.1538944,256 80.425166,253.493708 71.625166,248.787417 C62.825166,244.081125 55.9188745,237.174834 51.212583,228.374834 C46.5062915,219.574834 44,210.846106 44,186.7751 L44,109.2249 C44,85.1538944 46.5062915,76.425166 51.212583,67.625166 C55.9188745,58.825166 62.825166,51.9188745 71.625166,47.212583 C80.425166,42.5062915 89.1538944,40 113.2249,40 Z" id="path-1"></path>
                                        <filter x="-15.6%" y="-29.6%" width="131.3%" height="163.0%" filterUnits="objectBoundingBox" id="filter-2">
                                            <feOffset dx="0" dy="4" in="SourceAlpha" result="shadowOffsetOuter1"></feOffset>
                                            <feGaussianBlur stdDeviation="22" in="shadowOffsetOuter1" result="shadowBlurOuter1"></feGaussianBlur>
                                            <feColorMatrix values="0 0 0 0 0   0 0 0 0 0   0 0 0 0 0  0 0 0 0.264605978 0" type="matrix" in="shadowBlurOuter1"></feColorMatrix>
                                        </filter>
                                        <filter x="-12.6%" y="-23.6%" width="125.3%" height="150.9%" filterUnits="objectBoundingBox" id="filter-3">
                                            <feGaussianBlur stdDeviation="11" in="SourceAlpha" result="shadowBlurInner1"></feGaussianBlur>
                                            <feOffset dx="0" dy="0" in="shadowBlurInner1" result="shadowOffsetInner1"></feOffset>
                                            <feComposite in="shadowOffsetInner1" in2="SourceAlpha" operator="arithmetic" k2="-1" k3="1" result="shadowInnerInner1"></feComposite>
                                            <feColorMatrix values="0 0 0 0 0   0 0 0 0 0   0 0 0 0 0  0 0 0 0.194774683 0" type="matrix" in="shadowInnerInner1" result="shadowMatrixInner1"></feColorMatrix>
                                            <feGaussianBlur stdDeviation="2" in="SourceAlpha" result="shadowBlurInner2"></feGaussianBlur>
                                            <feOffset dx="0" dy="0" in="shadowBlurInner2" result="shadowOffsetInner2"></feOffset>
                                            <feComposite in="shadowOffsetInner2" in2="SourceAlpha" operator="arithmetic" k2="-1" k3="1" result="shadowInnerInner2"></feComposite>
                                            <feColorMatrix values="0 0 0 0 0   0 0 0 0 0   0 0 0 0 0  0 0 0 0.184612772 0" type="matrix" in="shadowInnerInner2" result="shadowMatrixInner2"></feColorMatrix>
                                            <feMerge>
                                                <feMergeNode in="shadowMatrixInner1"></feMergeNode>
                                                <feMergeNode in="shadowMatrixInner2"></feMergeNode>
                                            </feMerge>
                                        </filter>
                                    </defs>
                                    <g id="Page-1" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                                        <g id="iphone-copy">
                                            <use fill="black" fill-opacity="1" filter="url(#filter-2)" xlink:href="#path-1"></use>
                                            <use :fill="[like.coloring]" fill-rule="evenodd" xlink:href="#path-1"></use>
                                            <use fill="black" fill-opacity="1" filter="url(#filter-3)" xlink:href="#path-1"></use>
                                        </g>
                                    </g>
                                </svg>
                
                </li>

            </ul>

    </div>
</template>

<script>
export default {

    data() {
        
        return {

            likes: [{
                
                number:'1',

                coloring: ''

            }],

            visible1:true,
            visible:true,
            coloring:''

        }

    },

    methods:{
   
        toggleLike: function () {

            this.visible1 = !this.visible1
            var url = window.location.hash

        },
        
        addLike () {

            this.likes.push({

                number:'1',

                coloring: window.location.hash

            })

            console.log("yepaa : "+window.location.hash)

            

        },

        deleteLike () {

            this.likes.push({

                number:'1',

                coloring: window.location.hash

            })

            console.log("Nooope")

            

        },

        yesToggle: function () {

            this.toggleLike();
                    
            this.addLike();
            
        },

        noToggle: function () {

            this.toggleLike();
                    
            this.deleteLike();
            
        },

        Toggle: function () {

            this.visible = !this.visible
            var letters = '0123456789ABCDEF'
            var color = '#'
            for (var i = 0; i < 6; i++) {

                color += letters[Math.floor(Math.random() * 16)]

            }
            this.coloring = color;
            window.location = color;
            if(this.visible1){

            }else{

                this.visible1 = !this.visible1

            }
            
        },

        copyClip: function () {
            copyToClipboard("hola")
            console.log("copieur1")
            
        },
        
        copyToClipboard: function (element) {
        var temp = $("<input>")
        $("body").append(temp)
        temp.val(element).select()
        document.execCommand("copy")
        temp.remove()
        console.log("copieur2")
    }

    }

}
    


</script>

</script>
<style src="./like.css" >





</style>


