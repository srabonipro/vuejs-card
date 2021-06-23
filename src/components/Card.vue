<template>
    <div>
        <div class="the-card">
            <div class="the-card__title">
                <slot name="header">
                    <h2>Card Title</h2>
                </slot>
            </div>
            <div class="the-card__body">
                <slot name="body">
                    <img src="https://randomuser.me/api/portraits/men/78.jpg" alt="">
                    <p>
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Mollitia explicabo necessitatibus voluptas ex rerum alias fugit ea dicta facilis, maxime quas odit eius, voluptatibus pariatur modi. Corporis aut debitis deserunt.
                    </p>
                </slot>
            </div>
            <div class="the-card__footer" v-if="$slots.footer">
                <slot name="footer">
                    <a href="google.com">Learn More</a>
                </slot>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Card',
        mounted() {
            console.log(this.$slots);
        }
    }
</script>

<style>
.the-card {
    width: 500px;
    border: 1px solid #006f88;
    min-height: 200px;
    margin: 22px auto;
}
.the-card__title {
    background: #167db1;
    padding: 5px 11px;
    color: #fff;
}
.the-card__body {
    padding: 11px;
}
.the-card__body img {
    height: 150px;
}
ul {
    list-style-type: none;
    margin-right: 25px;
}
.the-card__footer {
    background: #e3e3e3;
    padding: 5px 11px;
    text-align: center;
}

</style>