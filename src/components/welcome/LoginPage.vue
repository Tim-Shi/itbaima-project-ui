<script setup>
import {Lock, User} from "@element-plus/icons-vue";
</script>

<template>
    <div style="text-align: center;margin: 0 20px;">
        <div style="margin-top: 120px;">
            <div style="font-size: 25px;font-weight: bold;">登录</div>
            <div style="font-size: 14px;color: gray;">在进入系统之前请先输入用户名和密码进行登录</div>
        </div>
        <div style="margin-top: 50px">
            <el-input type="text" placeholder="用户名/邮箱">
                <template #prefix>
                    <el-icon>
                        <User/>
                    </el-icon>
                </template>
            </el-input>
            <el-input type="password" style="margin-top: 10px;" placeholder="密码">
                <template #prefix>
                    <el-icon>
                        <Lock/>
                    </el-icon>
                </template>
            </el-input>
        </div>
        <el-row style="margin-top: 5px">
            <el-col :span="12" style="text-align: left">
                <el-checkbox v-model="checked1" label="记住我"/>
            </el-col>
            <el-col :span="12" style="text-align: right ">
                <el-link>忘记密码？</el-link>
            </el-col>
        </el-row>
        <div style="margin-top: 40px;">
            <el-button style="width: 270px;" type="success" plain>登陆</el-button>
        </div>
        <el-divider>
            <span style="color: grey;font-size: 13px;">没有账户</span>
        </el-divider>
        <div style="margin-top: 25px;">
            <el-button style="width: 270px;" type="warning" plain>注册</el-button>
        </div>
    </div>
</template>

<style scoped>

</style>