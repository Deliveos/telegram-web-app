<script lang="ts">
</script>

<div class="item">
    <slot/>
</div>

<style>
    .item {
        background-color: var(--tg-theme-secondary-bg-color);
        border-radius: 20px;
        display: flex;
        justify-content: center;
        align-items: center;
        box-sizing: border-box;
        width: 100%;
        height: 100%;
    }
</style>