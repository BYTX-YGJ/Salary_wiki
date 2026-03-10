# [**项目工资计算**](http://121.28.192.238:8562/salary/projectPay/projectSalaryCalculation)

## 一、总体流程

![image-20260310101647485](https://gitee.com/bytxrl/wiki-images/raw/master/image-20260310101647485.png)

按照项目组、岗位、业务线（可选）维护对应应出勤、计算规则、工资标准；依据"考勤汇总"、"考勤汇总（转岗）中信息生成对应工资标准、应出勤、计算规则（<span style='color:red;background:;font-size:文字大小;font-family:字体;'>没有维护考勤的无法生成</span>）；

在有业务线维护时，通过"[薪酬管理/项目工资/项目工资计算/业务线条/业务线条维护](http://121.28.192.238:8562/salary/projectPay/projectSalaryCalculation/BusinessLineName)"将人与业务线相绑定；

对应其它的绩效数据需要发送对应工资复核人审核通过后，导入系统并审批通过；

信息生成至个人后，"[薪酬管理/项目工资/项目工资计算/工资计算结果/工资查询](http://121.28.192.238:8562/salary/projectPay/projectSalaryCalculation/FirstSalaryInquiry)"，计算个人、项目组、月份的基础工资

## [**二、工资标准**](http://121.28.192.238:8562/salary/projectPay/projectSalaryCalculation/SalaryStandardTemplate)

1、首先按照项目、岗位、年月、业务类型维护对应的工资标准，维护好后找对应工资复核对接人审批，已审批通过的次月自动生成无需重复维护（例如：3月4号审批通过了2月的对应数据，那么4月1号会根据已审批通过的2月数据生成3月的工资标准）

![image-20260309150427228](https://gitee.com/bytxrl/wiki-images/raw/master/image-20260309150427228.png)

2、审批通过后的数据点击生成按钮会将工资标准生成至对应人身上

![image-20260310093617066](https://gitee.com/bytxrl/wiki-images/raw/master/image-20260310093617066.png)

## [**三、应出勤**](http://121.28.192.238:8562/salary/projectPay/projectSalaryCalculation/AttendanceTemplate)

1、首先按照项目、岗位、年月、业务类型维护对应的应出勤，维护好后找对应工资复核对接人审批，已审批通过的次月自动生成无需重复维护（例如：3月4号审批通过了2月的对应数据，那么4月1号会根据已审批通过的2月数据生成3月的应出勤）

![image-20260310093720718](https://gitee.com/bytxrl/wiki-images/raw/master/image-20260310093720718.png)

2、应出勤维护区分四种类别，法定出勤、月休天数、月出勤天数、考勤汇总的应出勤+哺乳假、固定出勤小时数

（1）选择法定出勤后，生成时应出勤小时数为每月法定天数*项目岗位标准工时

（2）选择月休天数后，生成时应出勤小时数为（每月天数-月休天数）*项目岗位标准工时

（3）选择月出勤天数后，生成时应出勤小时数为月出勤天数*项目岗位标准工时

（4）选择考勤汇总的的应出勤+哺乳假后，应特殊注意项目排班是否正确、每月单独维护入离职人员的应出勤

（5）固定出勤小时数

项目岗位标准工时查看路径：[薪酬管理/考勤管理/考勤规则设置/项目工时折算标准](http://121.28.192.238:8562/salary/attend/attendancerulesettings)

![image-20260310093808295](https://gitee.com/bytxrl/wiki-images/raw/master/image-20260310093808295.png)

3、审批通过后的数据点击生成按钮会将工资标准生成至对应人身上![image-20260310101954278](https://gitee.com/bytxrl/wiki-images/raw/master/image-20260310101954278.png)

## [**四、其它绩效数据**](http://121.28.192.238:8562/salary/projectPay/projectSalaryCalculation/OtherPerformanceData)

将以下涉及的内容，上传至薪酬管理/项目工资/项目工资计算/其它绩效数据，注意上传时，员工岗位与项目要与薪酬系统保持一致，否则无法读取，（例如：当月员工A在项目B担任话务员岗位，在项目C担任组长岗位，那么在上传其它绩效数据时，能正确读取的数据是员工A项目B话务员，员工A项目C组长；如果上传员工A项目B组长的数据，那么该条数据无法被读取）

![image-20260310100820414](https://gitee.com/bytxrl/wiki-images/raw/master/image-20260310100820414.png)

![image-20260310100347152](https://gitee.com/bytxrl/wiki-images/raw/master/image-20260310100347152.png)

## [**五、工资计算结果**](http://121.28.192.238:8562/salary/projectPay/projectSalaryCalculation/FirstSalaryInquiry)

![image-20260310100941207](https://gitee.com/bytxrl/wiki-images/raw/master/image-20260310100941207.png)

## 六、常见问题
