
<template>
    <header class="header" id='header'>
        <h1 id='siteName'>
            <a href=''>
                <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAeAAAABMCAYAAAC1fWS0AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAyNpVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADw/eHBhY2tldCBiZWdpbj0i77u/IiBpZD0iVzVNME1wQ2VoaUh6cmVTek5UY3prYzlkIj8+IDx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IkFkb2JlIFhNUCBDb3JlIDUuNS1jMDIxIDc5LjE1NDkxMSwgMjAxMy8xMC8yOS0xMTo0NzoxNiAgICAgICAgIj4gPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4gPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9IiIgeG1sbnM6eG1wPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvIiB4bWxuczp4bXBNTT0iaHR0cDovL25zLmFkb2JlLmNvbS94YXAvMS4wL21tLyIgeG1sbnM6c3RSZWY9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC9zVHlwZS9SZXNvdXJjZVJlZiMiIHhtcDpDcmVhdG9yVG9vbD0iQWRvYmUgUGhvdG9zaG9wIENDIChNYWNpbnRvc2gpIiB4bXBNTTpJbnN0YW5jZUlEPSJ4bXAuaWlkOkNBNzhBQzI0MERCQTExRTVCMzY0RTY1NENDQTdFQzk1IiB4bXBNTTpEb2N1bWVudElEPSJ4bXAuZGlkOkNBNzhBQzI1MERCQTExRTVCMzY0RTY1NENDQTdFQzk1Ij4gPHhtcE1NOkRlcml2ZWRGcm9tIHN0UmVmOmluc3RhbmNlSUQ9InhtcC5paWQ6Q0E3OEFDMjIwREJBMTFFNUIzNjRFNjU0Q0NBN0VDOTUiIHN0UmVmOmRvY3VtZW50SUQ9InhtcC5kaWQ6Q0E3OEFDMjMwREJBMTFFNUIzNjRFNjU0Q0NBN0VDOTUiLz4gPC9yZGY6RGVzY3JpcHRpb24+IDwvcmRmOlJERj4gPC94OnhtcG1ldGE+IDw/eHBhY2tldCBlbmQ9InIiPz7Hej/oAAAOlklEQVR42uydS27j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" />
            </a>
        </h1>
        <nav class="nav">
            <ul>
                <li v-for="(val,index) of nav" v-bind:key="index">{{ val }}</li>
            </ul>
        </nav>
    </header>
</template>

<script>
    const Header =  {
        template: '#header',
        data:function(){
            return {
                nav: [
                    'Home',
                    'Artcle',
                    'Garden',
                    'Travel',
                    'Work'
                ]
            }
        }
    }
    export default Header;
</script>

<style scoped>

    #header {
        position: relative;
        width: 100%;
        height: 70px;
        color: blue;
        font-size: 24px;
        box-sizing: border-box;
    }
    #header .nav {
        width: 100%;
        height: 100%;
    }
    #header .nav ul {
        width: 100%;
        height: 100%;
        margin: 0;
        padding: 0 0 0 15%;
    }
    #header .nav li {
        float: left;
        font-size: 13px;
        padding: 28px 10px;
        line-height: 1;
        list-style: none;
        color: #000;
    }
    #siteName {
        z-index: 1001;
        top: 0;
        left: 0;
        margin: 0;
        position: absolute;
        width: 130px;
    }
    #siteName a {
        padding: 15px 0;
        display: block;
        line-height: 1;
    }
    #siteName img {
        width: 100%;
        height: auto;
        vertical-align: middle;
    }
</style>