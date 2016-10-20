<template>
    <!-- Navigation -->
    <nav id="nav" class="navbar navbar-default navbar-static-top" role="navigation" style="margin-bottom: 0">
        <div class="navbar-header">
            <a class="navbar-brand" href="index.html">监控管理后台</a>
        </div>
        <!-- /.navbar-header -->

        <ul class="nav navbar-top-links navbar-right">
            <li>
                <a v-on:click="logout" v-link="{ path: '/login', replace: true }"> <i class="fa fa-sign-out fa-fw" ></i> 登出 </a>
            </li>
        </ul>
        <!-- /.navbar-top-links -->
    </nav>

	<!-- main view -->
	<router-view></router-view>
</template>

<style type="text/css">
	.navbar-right {
		margin-right: 0;
	}
	.nav>li>a {
		padding: 15px;
	}
</style>

<script>
export default {
	data () {
		return {
			msg: 'Hello from vue-loader!cghsdfg'
		}
	}
}
</script>