<script>
    import leafLogo from "../assets/leaf.static.png";
    import capsuleLogo from "../assets/capsule.static.png";
    import tadm from "../assets/tadm.png";

</script>



<div class="container relative max-w-6xl m-auto flex items-center justify-start h-[95vh]">


   <!-- <svg class="absolute opacity-20  w-full h-full bg-center"  xmlns="http://www.w3.org/2000/svg" version="1.1" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:svgjs="http://svgjs.dev/svgjs" viewBox="0 0 800 400"><path d="M0.8968609571456909,397.3094177246094C0.8968609571456909,397.3094177246094,100.44843292236328,239.46188354492188,100.44843292236328,239.46188354492188C100.44843292236328,239.46188354492188,275.3363342285156,324.6636657714844,275.3363342285156,324.6636657714844C275.3363342285156,324.6636657714844,421.524658203125,157.8475341796875,421.524658203125,157.8475341796875C421.524658203125,157.8475341796875,554.2600708007812,331.83856201171875,554.2600708007812,331.83856201171875C554.2600708007812,331.83856201171875,799.1031494140625,50.22421646118164,799.1031494140625,50.22421646118164" fill="none" stroke-width="1" stroke="url(&quot;#SvgjsLinearGradient1002&quot;)" stroke-linecap="round" stroke-opacity="1"></path><defs><linearGradient id="SvgjsLinearGradient1002" gradientTransform="rotate(0, 0.5, 0.5)"><stop stop-color="hsl(1, 69%, 60%)" offset="0"></stop><stop stop-color="hsl(205, 91%, 80%)" offset="1"></stop></linearGradient></defs></svg> -->
   <div class="w-full  lg:grid grid-cols-2 relative">

   


    <div class="w-full flex justify-center items-center">
      <div class="p-4 space-y-20 ">

        <div class="text-2xl lg:text-6xl mb-2 ubuntubold" style="line-height: 1.2;">
         <span class="relative">BOOST YOUR <div class="w-full lg:h-6 h-2 bg-green-200 absolute bottom-0" style="z-index: -1;"></div></span> PRODUCTIVITY

          <div class="text-2xl lg:text-6xl 
          mb-2 text-gray-400 font-thin ubuntuthin" style="line-height: 1.2;">
              BE BETTER VERSION OF YOURSELF
            </div>

            <div class=" text-lg">
              Coming Soon
            </div>
        </div>

       
  
        <div class="flex space-x-1 ">
          <img class="-rotate-45" width="50"  src="{leafLogo}" alt="">
          <div class="lg:text-2xl">
            <h1 class="font-bold">100%</h1> 
            <p class="text-gray-500">VEGAN</p>
           </div>
        </div>
     
        <a class="text-2xl text-blue-700 uppercase " on:click={hideModal=false} href="/">Preorder now 🤝</a>
      </div>


  
    </div>

    <div class="relative">

      <div class="relative">

        <img class="absolute bottom-16 right-[35%] z-10 animate-floating " width="120" src="{capsuleLogo}" alt="">
        <img class="absolute top-[50%] left-20 -rotate-45 z-10 blur-sm animate-floating " width="60" src="{capsuleLogo}" alt="">
        <img class="absolute top-[30%] left-20 -rotate-45  blur-sm animate-floating " width="70" src="{capsuleLogo}" alt="">
        <img class="absolute top-[10%] left-[30%] -rotate-45  blur-md animate-floating " width="30" src="{capsuleLogo}" alt="">
        <img class="absolute top-40 right-40 -rotate-45  animate-floating " width="70" src="{capsuleLogo}" alt="">
        <!-- <img class="absolute top-[50%] right-20 rotate-45 animate-floating" width="90" src="{capsuleLogo}" alt=""> -->
        <img class="absolute blur-sm top-[50%] right-[30%] -rotate-45  animate-floating " width="90" src="{capsuleLogo}" alt="">
        
        <img
        src="{tadm}"
        alt=""
        width="300"
        loading="lazy"
        class="object-cover object-center rotate-12 m-auto"
      >
      </div>


  

    </div>
  </div>
</div>
