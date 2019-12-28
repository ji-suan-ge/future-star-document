# 小程序
## 报名Page:Apply
### 查看创业营列表Component:\<CampItem(v-for)\>
#### 查看创业营信息Page:CampInfo/Component:img+p
#### 查看每期创业营的班级列表Page:CampInfo/Component:\<ClassItem v-for="applyList"\>
* 查看班级介绍信息Page:ClassInfo/Component:img+p
* 查看班级中的校友 ?
* 填写班级报名信息表单Page:ClassInfo/Component:applyForm

## 班级Page:Class
### 查看正在进行的班级列表Navigator:ongoing/Component:\<ClassItem v-for="ongoingList"\>
* 查看课程信息Page:ClassInfo/Navigator:course/Component:\<CourseItem v-for="ongoingClass"\>
	* 查看老师名片（头像、姓名、头衔、联系方式）Page:CourseInfo/Component:?
	* 查看课程信息（时间、地点）Page:CourseInfo/Component:p
	* 查看课程资料 Page:CourseInfo/Component:\<ResourceItem v-for="resourceList"\>
* 查看同学列表Page:ClassInfo/Navigator:classmate/Component:\<SchoolmateItem v-for="classmateList"\>
* 查看班级介绍Page:ClassInfo/Navigator:info/Component:img+p
### 查看正在审核的班级列表Navigator:auditing/Component:\<ClassItem v-for="auditList"\>
* 查看审核状态Page:ClassInfo/Navigator:auditState/Component:icon+span||步骤条
* 查看评价信息Page:ClassInfo/Navigator:comment/Component:p
* 查看班级介绍Page:ClassInfo/Navigator:info/Component:img+p
### 查看已经结束的班级列表Navigator:finished/Component:\<ClassItem v-for="finishedList"\>
* 查看课程信息Page:ClassInfo/Navigator:course/Component:<CourseItem v-for="ongoingClass">
	* 查看老师名片（头像、姓名、头衔、联系方式）Page:CourseInfo/Component:?
	* 查看课程信息（时间、地点）Page:CourseInfo/Component:p
	* 查看课程资料 Page:CourseInfo/Component:\<ResourceItem v-for="resourceList"\>
* 查看同学列表Page:ClassInfo/Navigator:classmate/Component:\<SchoolmateItem v-for="classmateList"\>
* 查看班级介绍Page:ClassInfo/Navigator:info/Component:img+p

## 校友Page:Schoolmate
### 搜索校友Component:button
### 按期查看校友Component:
### 按拼音序查看校友列表Component:\<SchoolmateItem v-for="schoolmateList"\>
#### 查看校友信息Page:SchoolmateInfo 表单内容详见我的

## 活动Page:Activity
### 查看正在报名和等待报名的活动Navigator:hot
#### 热门活动轮播
* 正在报名活动列表Navigator:ongoing/Component:\<ActivityItem v-for="ongoingList"\>
	* Page:ActivityInfo
	* 活动信息（主办单位、时间地点、活动日程、参赛人群、收费标准、报名时间、报名上限）Component:\<p\>
	* 确认活动弹框并缴费
* 等待报名活动列表Navigator:await/Component:\<ActivityItem v-for="awaitList"\>
	* Page:ActivityInfo
	* 活动信息（主办单位、时间地点、活动日程、参赛人群、收费标准、报名时间、报名上限）Component:\<p\>
	* 报名按钮禁用（活动未开始）
### 查看往期活动Navigator:finished
* 往期活动列表Component:\<ActivityItem v-for="finishedList"\>
	* Page:ActivityInfo
	* 活动信息（主办单位、时间地点、活动日程、参赛人群、收费标准、报名时间、报名上限）Component:\<p\>
	* 报名按钮禁用（活动已结束）
### 查看我参与的活动Navigator:mine
* 已报名活动列表Navigator:applied/Component:\<ActivityItem v-for="appliedList"\>
	* Page:ActivityInfo
	* 活动信息（主办单位、时间地点、活动日程、参赛人群、收费标准、报名时间、报名上限）Component:\<p\>
	* 报名按钮禁用（活动已报名）
	* 点击查看参与校友列表 Component:\<button\>
		* Page: activitySchoolmate/Component:<SchoolmateItem v-for="activitymateList">
			* 查看校友详细信息 Page:SchoolmateInfo
* 往期活动列表Navigator:finished/Component:<ActivityItem v-for="finishedList">
	* Page:ActivityInfo
	* 活动信息（主办单位、时间地点、活动日程、参赛人群、收费标准、报名时间、报名上限）Component:\<p\>
	* 报名按钮禁用（活动已结束）
	* 点击查看参与校友列表 Component:\<button\>
		* Page: activitySchoolmate/Component:\<SchoolmateItem v-for="activitymateList"\>
			* 查看校友详细信息 Page:SchoolmateInfo

## 我的Navigator:Mine
### 查看我的信息Page:MineInfo
#### 编辑我的信息Component:\<button\>
* Page:EditMineInfo
* 填写表单form
* 提交表单