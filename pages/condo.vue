
<template>
    <div>
      <div class="py-6 select-none bg-red-500">
        <h1 class="text-xl font-semibold text-center text-white sm:text-2xl">
          <!--The white coloured text rename to desired Main title. will be displayed on the page-->
          Floor Plan @ Place Name
        </h1>
      </div>
      <div class="max-w-4xl px-2 mx-auto space-y-6 divide-y">
       <!-- Facilities  -->
       <!-- The white coloured text will be displayed on your page. Rename accordingly to your requirements-->
       <!-- Check file components>Design.vue file line 67 for next step-->
        <section  class="py-6 space-y-6">
            <div class="space-y-4">
            <h3 class="text-xl font-semibold sm:text-2xl">Facilities </h3>
            <section>
        <div class="max-w-6xl px-4 py-12 mx-auto space-y-12">
          <div class="space-y-4">
            <h3 class="text-xl font-semibold sm:text-2xl text-center">
              1 bedroom 
            </h3>
            <!-- You can rename LayoutOneBedroom to your desired variable name
            example: rename "LayoutOneBedroom" on line 27 to "MallLGFloor". DON'T forget to rename LayoutOneBedroom on line 72 to MallLGFloor too
            Do the same to the rest if you are required to rename it. For example "LayoutTwoBedroom" on line 33 and line 79-->
            <Design :floor-plan-prop="LayoutOneBedroom" />
          </div>
          <div class="space-y-4">
            <h3 class="text-xl font-semibold sm:text-2xl text-center">
              2 bedroom
            </h3>
            <Design :floor-plan-prop="LayoutTwoBedroom" />
          </div>
          <div class="space-y-4">
            <h3 class="text-xl font-semibold sm:text-2xl text-center">
              3 bedroom
            </h3>
            <Design :floor-plan-prop="LayoutThreeBedroom" />
          </div>
          <div class="space-y-4">
            <h3 class="text-xl font-semibold sm:text-2xl text-center">
              4 bedroom
            </h3>
            <Design :floor-plan-prop="LayoutFourBedroom" />
          </div>
          <div class="space-y-4">
            <h3 class="text-xl font-semibold sm:text-2xl text-center">
              5 bedroom
            </h3>
            <Design :floor-plan-prop="LayoutFiveBedroom" />
          </div>
        </div>
      </section>
          </div>
        </section> 
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        //Please rename the title (orange coloured text) and url (orange coloured text) below to the intended title and images
        //the title will be displayed on the page and
        //url needs to use the same name with the name of the pictures you put in the assets>img>create your-own-folder (to hold the pictures)
        //example; for this template, we have a folder named floorlayout. 
        //floorlayout folder have a picture named: Layout1.jpg so the url part below will be url: 'Layout1'
        //so if you create your-own-folder named: shoplots, and import all the pictures into the folder the steps will be the same
        //example: assets>img>shoplots>watson.jpg, the title will be, title: 'Watson' and url will be, url: 'watson' 

        //You can add and remove the number of layout below according to your requirements. 
        //delete the whole line if not needed, and add the whole line if needed. example on LayoutFourBedroom and LayoutFiveBedroom
        LayoutOneBedroom: [
          { title: 'LayoutOne1', url: 'Layout1' },
          { title: 'LayoutOne2', url: 'Layout2' },
          { title: 'LayoutOne3', url: 'Layout3' },
          { title: 'LayoutOne4', url: 'Layout4' },
          { title: 'LayoutOne5', url: 'Layout5' },
        ],
        LayoutTwoBedroom: [
          { title: 'LayoutTwo1', url: 'Layout1' },
          { title: 'LayoutTwo2', url: 'Layout2' },
          { title: 'LayoutTwo3', url: 'Layout3' },
          { title: 'LayoutTwo4', url: 'Layout4' },
          { title: 'LayoutTwo5', url: 'Layout5' },
        ],
        LayoutThreeBedroom: [
          { title: 'LayoutThree1', url: 'Layout1' },
          { title: 'LayoutThree2', url: 'Layout2' },
          { title: 'LayoutThree3', url: 'Layout3' },
          { title: 'LayoutThree4', url: 'Layout4' },
          { title: 'LayoutThree5', url: 'Layout5' },
        ],
        LayoutFourBedroom: [
          { title: 'LayoutFour1', url: 'Layout1' },
          { title: 'LayoutFour2', url: 'Layout2' },
          { title: 'LayoutFour3', url: 'Layout3' },
          { title: 'LayoutFour4', url: 'Layout4' },
        ],
        LayoutFiveBedroom: [
          { title: 'LayoutFive1', url: 'Layout1' },
          { title: 'LayoutFive2', url: 'Layout2' },
          { title: 'LayoutFive3', url: 'Layout3' },
        ],

      }
    },
  }
  </script>
  