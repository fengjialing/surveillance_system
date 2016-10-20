<template>
    <div class="container">
    	<dl>
    		<dt>mysql服务</dt>
    		<dd>服务1描述</dd>
    	</dl>
    	<h4>服务应用</h4>
    	<table class="table table-bordered table-hover">
    		<tr class="info">
    			<th>应用名称</th>
    			<th>应用描述</th>
    			<th>主机IP</th>
    			<th>主机端口</th>
    			<th>操作</th>
    		</tr>
    		<tr v-for="app in appList">
    			<td>{{ app.name }}</td>
    			<td>{{ app.der }}</td>
    			<td>{{ app.IP }}</td>
    			<td>{{ app.n }}</td>
    			<td>
    				<button type="button" class="btn btn-default">编辑应用</button>
    				<button type="button" class="btn btn-default">应用详情</button>
    				<button type="button" class="btn btn-default">取消关联该应用</button>
    			</td>
    		</tr>
    	</table>
    </div>
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