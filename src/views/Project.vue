<template>
    <div class="project">
        <b-card-group column class="p-3">
            <b-card no body id="card-project">
                <b-card-img img-top :src="require('../assets/project/portfolio.png')" alt="Image" class="rounded-0"></b-card-img>
                <b-card-body title="GC Official Website">
                    <b-card-text>
                        Offical Website of Gilchrist Calunia<br>
                        Contributors : GC & VeoScript & Acatzk<br>
                        -Written in Bootstrap Vue
                    </b-card-text>
                    <b-button pill variant="success" id="btngithub" href="https://github.com/Gilchrist32/gilchristcalunia-portfolio" target="_blank" size="md">
                    <b-icon size="sm" class="ml-1 mt-0 mr-3" icon="files" aria-hidden="true"></b-icon>View on Github</b-button>
                </b-card-body>
            </b-card>
        </b-card-group>
    </div>
</template>
<style scoped>
 .projects{
    margin-top: 90px;
  }
  #card-project{
    background: #20284D;
    color: #A8B3DB;
  }
  .card-title{
    font-size: 25px;
    font-weight: bolder;
    color: #fff;
  }
  

</style>>