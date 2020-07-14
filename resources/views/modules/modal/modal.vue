<template>
    <transition name="modal" mode="in-out">
        <div class="modal" v-if="show">
            <div class="modal__mask" @click="close"></div>
            <div class="modal__box">
                <a class="modal__close">
                    <img src="/images/close.png" alt="img" @click="close">
                </a>
                
                <a class="btn"><span>Send Me The Tips »</span></a>
            </div>
        </div>
    </transition>
</template>

<script>
    export default {
        props: {
            show: {
                type: Boolean,
                required: true,
                default: false
            }
        },
        methods: {
            close () {
                this.$emit('close')
            }
        }
    }
</script>

<style lang="scss" scoped>
    .modal {
        display: flex;
        align-items: center;
        justify-content: center;
        position: fixed;
        top: 0;
        left: 0;
        height: 100%;
        width: 100%;
        
        &__close {
            position: absolute;
            top: 15px;
            right: 15px;
        }

        &__mask {
            position: absolute;
            top: 0;
            left: 0;
            height: 100%;
            width: 100%;
            background: rgba(38, 38, 38, 0.8);
            cursor: pointer;
        }

        &__box {
            position: relative;
            width: 570px;
            padding: 38px 65px;
            background: #fff;
        }
    }

    .modal-leave-active,
    .modal-enter-active {
        transition: all .4s linear;
        .modal__mask,
        .modal__box {
            transition: all .4s cubic-bezier(0.5, 0, 0.5, 1);
        }
    }

    .modal-enter, .modal-leave-to {
        .modal__mask {
            background: transparent;
        }
        .modal__box {
            opacity: 0;
            transform: translateY(-50px)
        }
    }
</style>