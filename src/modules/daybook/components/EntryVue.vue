<template>
<div 
    class="entry-container mb-3 pointer p-2"
    @click="$router.push({name: 'entry', params: { id: 10}})"
    >
    <div class="entry-title d-flex">
        <span class="text-success fs-5 fw-bold ">15</span>
        <span class="mx-1 fs-5">julio</span>
        <span class="mx-1 fw-light">2021, jueves</span>
    </div>
    <div class="entry-description">
        Dolore minim consequat aliqua reprehenderit nostrud. Sit aliqua sunt aliqua dolor. Ut deserunt consectetur fugiat sunt laboris sunt magna adipisicing est anim. Id cupidatat ut irure laboris nostrud enim velit Lorem et.
    </div>
</div>  
</template>

<!-- </script> -->

<style lang='scss' scope>
.entry-container {
    border-bottom: 1px solid #2c3e50;
    transition: 0.2s all ease-in;
    &:hover{
        background-color: lighten($color: grey, $amount: 45);
        transition: 0.2s all ease-in;
    }
    .entry-description{
        font-size: 12px
    }
}
</style>