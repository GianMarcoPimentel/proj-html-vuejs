<script>
export default {
  name:'AppStatistic',

  data() {
    return {
        statistics : [
            {
                scope: 'Successfully trained',
                number: '1790',
                action: 'enrolled learners',
            },
            {
                scope: 'Proudly Received',
                number: '19',
                action: 'countrywide awards',
            },
            {
                scope: 'Firmly Established',
                number: '24',
                action: 'local branches',
            },
            {
                scope: 'Getting Featured on',
                number: '1090',
                action: 'Blog Posts',
            },
            
        ]
    }
  },
}
</script>

<template>
    <div class="container">
        <div class="statistics">
            <div v-for="statistic in statistics"
            class="block"
            >
            <div class="scope">{{ statistic.scope }}</div>
            <div class="number">{{ statistic.number }}</div>
            <div class="action">{{ statistic.action }}</div>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
.statistics{
    width: 100%;
    display: flex;
    justify-content: space-between;
    padding: 40px 20px;

    .block{
        display: flex;
        flex-flow: column;
        align-items: center;
        justify-content: space-around;
        gap: 20px;
        
        .scope{
            color:#3F3A64;
            font-weight: bold;
        }
        .number{
            font-size: 20px;
            font-weight: bold;
            color: #20ad96;
        }
        .action{
            color: #908DA5;
            font-weight: bold;
            text-transform: uppercase;

        }
    }
}
</style>