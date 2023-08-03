<template>
    <div class="board">
        <div class="logo">
            <img src="@/assets/Logo.svg" alt="" />
        </div>
        <div class="right">
            <span class="lager">
                <img src="@/assets/SearchIcon.svg" alt="" />
                <span>Sign in</span>
                <button>Get started - it's free</button>
            </span>
            <span class="small">
                <img src="@/assets/HamburgerMenu.svg" alt="" />
            </span>
        </div>
    </div>
</template>
<style scoped>
.board {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100px;
}

.right {
    display: flex;
    justify-content: flex-end;
    align-items: center;
}
.right .lager {
    display: flex;
    gap: 25px;
    align-items: center;
}

.right .small {
    display: none;
}

@media (max-width: 568px) {
    .right .lager {
        display: none;
    }
    .right .small {
    display: inline-block;
}
}

</style>