<template>
  <div id="vizContainer">
  </div>
</template>

<script>
export default {
  name: 'TableauHolder',
  methods: {
        initViz () {
            const containerDiv = document.getElementById("vizContainer")
            
            let url = "http://public.tableau.com/views/RegionalSampleWorkbook/Storms"

            let options = {
                hideTabs: true,
                onFirstInteractive: () => { 

                }
            }
            
            this.viz = new window.tableau.Viz(containerDiv, url, options)
        }
    },
    mounted () {
        window.addEventListener('load', () => {
            this.initViz()
        })
    }
}
</script>


<style scoped>

</style>
