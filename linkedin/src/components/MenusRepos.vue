<template>
    <div class="repositorio col-md-9 col-sm-12">
        <ul class="menu list-inline">
            <li class="list-inline-item" v-on:click="setActive('repos')" :class="{ active: isActive('repos') }">Repos</li>
            <li class="list-inline-item" v-on:click="setActive('starred')" :class="{ active:isActive('starred') }">Starred</li>
        </ul>
    </div>
</template>

<script>
export default {
    data() {
        return { activeItem: 'about' }
    },
    methods: {
        isActive: function (menuItem) {
            return this.activeItem === menuItem
        },
        setActive: function (menuItem) {
            this.activeItem = menuItem 
        }
    }
}
</script>
<style lang="scss">
    @import "../scss/variaveis";
    .repositorio {
        color: $slate-grey-two;
        .menu.list-inline {
            border-bottom: 2px solid $white-two;
            margin-top: 30px;
            width: calc(100% + 15px);
            li {
                margin: 20px;
                &:nth-child(2) {
                    &:after {
                        content: "";
                        transition: all .2s ease;
                        border-bottom: 4px solid $rusty-orange;
                        width: 88px;
                        position: absolute;
                        top: 93px;
                        left: 15px;
                    }
                }
            }
            li.active {
                font-weight: bold;                
                &:nth-child(2) {
                    &:after {
                        width: 98px;
                        left: 101px;
                    }
                }
            }
        }
    }
</style>