<template>
    <div>
        <div class="md:py-16 bg-brand-red-light-1 text-center md:text-left flex flex-col md:flex-row border-b-2">
            <div v-for="stat in stats" :key="stat.category" class="py-11 md:py-0 md:px-11 border-b-2 md:border-b-0 md:border-r-2 border-brand-red-light-3 flex-grow">
                <h1 class="text-brand-gray-light">TOTAL NUMBER</h1>
                <h1 class="text-brand-gray-light">{{ stat.category }}</h1>
                <h1 class="text-brand-gray-dark-1 text-3xl">{{ stat.figure }}</h1>
            </div>
            <div class="py-11 md:py-0 md:px-11 border-brand-red-light-3 flex-grow">
                <h1 class="text-brand-gray-light">PARTICIPANT</h1>
                <h1 class="text-brand-gray-light">LOCATIONS</h1>
                <h1 class="text-brand-gray-dark-1">Lagos <br> And from around the world </h1>
            </div>   
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            stats: [
                {category: 'OF PARTICIPANT', figure: '2,056,789'},
                {category: 'OF FEMALE PARTICIPANT', figure: '1,578,789'},
                {category: 'OF MALE PARTICIPANT', figure: '900,789'}
            ]
        }
    }
}
</script>

<style scoped>

</style>