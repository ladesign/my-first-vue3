<template>

    <div class="todolist">
        <div class="todo_wrapper">
            <h1 style="border-bottom:1px dotted">To Do List</h1>
            <br>
            <div class="add_block">
                <input class="todo_input" type="text" placeholder="請輸入文字" />
                <button class="add_item">加入</button>
            </div>
            <div class="nav_block">
                <button class="nav_item">全部</button>
                <button class="nav_item">進行中</button>
                <button class="nav_item">已完成</button>
            </div>
            <ul class="todo_item">
                <li>
                    <button class="btn_icon" type="button" style="float:left">&#10004;</button>
                    <button class="btn_icon" type="button" style="float:left">&#9744;</button>
                    <label style="margin-left: 5px; cursor: pointer;"></label>
                    <button class="btn_icon" type="button" style="float:right">&#10008;</button>
                </li>
            </ul>
        </div>
    </div>

</template>

<style>
@media (min-width: 1024px) {
    .todolist {
        min-height: 100vh;
        display: flex;
        align-items: center;
    }
}
    li {
        width: 100%;
        height: 50px;
        list-style: none;
        background-color: #ffffff;
        padding: 13px;
        cursor: pointer;
    }

        li:hover {
            background-color: #cacaca;
        }


    .todo_wrapper {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        background-color: #ededed;
        height: 500px;
        width: 500px;
        border-radius: 5px;
    }

    .add_block {
        display: inline-flex;
        width: 85%;
        justify-content: space-around
    }

    .todo_input {
        border: none;
        outline-style: none;
        padding: .375rem .75rem;
        width: 85%;
    }

    .add_item {
        border: none;
        background-color: #808080;
        margin-left: 10px;
        color: aliceblue;
        cursor: pointer;
        padding: .375rem .75rem;
    }

    .nav_block {
        margin-top: 15px;
        border-bottom: 1px solid #808080;
        width: 85%
    }

    .nav_item {
        border: none;
        background-color: #ffffff;
        margin-left: 10px;
        color: #808080;
        cursor: pointer;
        padding: .375rem .75rem
    }

    .todo_item {
        width: 85%;
        height: 300px;
        overflow-y: auto;
        margin-top: 20px;
        scrollbar-width: thin;
        padding: inherit;
    }

    .btn_icon {
        background: none;
        border: none;
        cursor: pointer;
    }
</style>
