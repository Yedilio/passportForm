<template>
    <div class="modal">
        <div class="footer">
            <i
                    @click="$emit('isShow')"
                    class="material-icons">cancel</i>
        </div>
        <div class="content">
            Пользователь успешно создан!
        </div>
    </div>
</template>

<script>
    export default {
        name: "ModalWindows",
        props: {
            isShow: {
                type: Boolean
            }
        }
    }
</script>

<style lang="scss" scoped>
    .modal {
        height: 100px;
        width: 150px;
        display: flex;
        flex-direction: column;
        background-color: #808080;
        border: 1px solid black;

        position: absolute;
        z-index: 10;
        top: 50px;
        left: 35%;
        box-shadow: 0 0 17px 0 #e7e7e7;

        .footer {
            height: 34px;
            display: flex;
            align-items: center;
            justify-content: flex-end;
            padding: 5px 8px;
            background-color: #777;
        }

        .content {
            height: 100%;
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
        }
    }
</style>
