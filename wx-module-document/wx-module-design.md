# 小程序
## 报名Page:Enroll
### 查看创业营列表Component:CampItem(v-for)
#### 查看创业营信息Page:CampInfo/Component:img+p
#### 查看每期创业营的班级列表Page:CampInfo/Component:<ClassItem v-for="enrollList">
* 查看班级介绍信息Page:ClassInfo/Component:img+p
* 查看班级中的校友 ?
* 填写班级报名信息表单Page:ClassInfo/Component:EnrollForm
## 班级Page:Class
### 查看正在进行的班级列表Navigator:ongoing/Component:<ClassItem v-for="ongoingList">
* 查看课程信息Page:ClassInfo/Navigator:course/Component:<CourseItem v-for="ongoingClass">
	* 查看老师名片（头像、姓名、头衔、联系方式）Page:CourseInfo/Component:?
	* 查看课程信息（时间、地点）Page:CourseInfo/Component:p
	* 查看课程资料 Page:CourseInfo/Component:<ResourceItem v-for="resourceList">
* 查看同学列表Page:ClassInfo/Navigator:classmate/Component:<Schoolmate v-for="classmateList">
* 查看班级介绍Page:ClassInfo/Navigator:info/Component:img+p
### 查看正在审核的班级列表Navigator:auditing/Component:<ClassItem v-for="auditList">
* 查看审核状态Page:ClassInfo/Navigator:auditState/Component:icon+span||步骤条
* 查看评价信息Page:ClassInfo/Navigator:comment/Component:p
* 查看班级介绍Page:ClassInfo/Navigator:info/Component:img+p
### 查看已经结束的班级列表Navigator:finished/Component:<ClassItem v-for="finishedList">
* 查看班级介绍Page:ClassInfo/Component:img+p
* 查看审核状态Page:ClassInfo/Component:icon+span||步骤条
* 查看评价信息Page:ClassInfo/Component:p