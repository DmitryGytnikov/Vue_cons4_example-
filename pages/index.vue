<script setup></script>
<template>
	<div>hello i am</div>
	<Component1 />
	<el-button @click="ElMessage('hello')">button</el-button>
	<ElButton :icon="ElIconEditPen" type="success">button</ElButton>
	<LazyElButton type="warning">lazy button</LazyElButton>
	<div>
		<el-button-group>
			<el-button type="primary" :icon="ArrowLeft">Previous Page</el-button>
			<el-button type="primary">
				Next Page<el-icon class="el-icon--right"><ArrowRight /></el-icon>
			</el-button>
		</el-button-group>
	</div>
	<el-form-item label="Activity name">
		<el-input />
	</el-form-item>
	<el-popconfirm title="Are you sure to delete this?">
		<template #reference>
			<el-button>Delete</el-button>
		</template>
	</el-popconfirm>
</template>
