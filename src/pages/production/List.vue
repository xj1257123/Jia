<template>
    <div>
        <h1>产品管理</h1>
        <el-button type="success" size="small">添加</el-button>
        <el-button type="danger" size="small">删除</el-button>
        <el-table>
            <el-table-column prop="id" label="编号"></el-table-column>
            <el-table-column prop="name" label="产品名称"></el-table-column>
            <el-table-column label="价格"></el-table-column>
            <el-table-column label="描述"></el-table-column>
            <el-table-column label="所属产品"></el-table-column>
            <el-table-column label="操作">
                <template v-slot="slot">
                <a href="">删除</a>
                <a href="">修改</a>
                </template>
            </el-table-column>
        </el-table>
        <div class="block">
  <el-pagination
    layout="prev, pager, next"
    :total="50">
  </el-pagination>
</div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>

</style>