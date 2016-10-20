<template>
	<h4>应用列表</h4>
	<button type="button" class="btn btn-primary btn-lg">新建应用</button>
	<table class="table table-bordered table-hover">
		<tr class="info">
			<th>应用名</th>
			<th>应用描述</th>
			<th>IP</th>
			<th>端口</th>
			<th>操作</th>
		</tr>
		<tr v-for="app in appList">
			<td>{{ app.name }}</td>
			<td>{{ app.der }}</td>
			<td>{{ app.IP }}</td>
			<td>{{ app.n }}</td>
			<td>
				<a v-link="{path:'/editApplication'}" type="button" class="btn btn-default">编辑</a>
				<button type="button" class="btn btn-default">应用详情</button>
				<button type="button" class="btn btn-default">删除</button>
			</td>
		</tr>
	</table>
</template>

<script>
	
    export default {
        data(){
            return{
                appList:[{
                	name: "sql主",
                	der: "MySQL主节点",
                	IP: "194.168.42.12",
                	n: 3306,
                }
                ]
            }
        },
        components:{
            
        },
        methods:{
            
        },
        events:{
        }
    }

</script>