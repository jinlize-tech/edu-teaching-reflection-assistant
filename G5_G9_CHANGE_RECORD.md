# G5/G9 产品修改记录

- 产品编号：$(@{number=41; product_id=JLZ-EDU-SK-035; chinese_name=教学反思助手; english_name=Teaching Reflection Assistant; repository_name=edu-teaching-reflection-assistant; repository_url=https://github.com/jinlize-tech/edu-teaching-reflection-assistant; product_type=Skill; category_code=03; category=03 教学教研中心; description=课堂教学反思和改进建议。; target_users=System.Object[]; core_input=课堂事实记录、教学目标、学生反应、教师困惑和同事反馈; main_output=事实与判断分离的反思、问题排序、改进实验和下次观察点; product_risk=把自我评价当事实或空泛鼓励; dedup_label=存在部分功能交叉; dedup_note=与教师成长反馈专家区分：单次课堂反思，不承担长期成长评估和教练式反馈。; development_status=Planned / 待研发; license=Apache-2.0; spec_version=1.0.0; workbuddy_status=PLANNED_FOR_WORKBUDDY}.product_id)
- 产品名称：教学反思助手
- 基线：EDUCATION_BASELINE_V1.0.0
- 基线提交：$BaselineCommit
- 原版本：1.0.0
- 新版本：1.0.1

## 本次修改

1. 强化产品专属执行流程、输入核对和输出验收规则。
2. 新增 scripts/validate_input.js，实际检查必填字段、冲突、未确认数据和敏感信息。
3. 新增正常、缺失、冲突、敏感信息和非法JSON场景输入。
4. 测试升级为 T1–T7 分层并保存逐项检查结果。
5. 安装包加入 Apache-2.0 LICENSE 和 THIRD_PARTY_NOTICES.md。
6. 安装包升级为 1.0.1，加入许可证、第三方声明和输入校验脚本，保留 1.0.0 ZIP。
7. 按本产品冻结规格补充专属处理规则、输入到成果的核对矩阵和去重边界。

## 产品专属增强

- 核心任务：课堂教学反思和改进建议。
- 主要风险：把自我评价当事实或空泛鼓励
- 去重边界：与教师成长反馈专家区分：单次课堂反思，不承担长期成长评估和教练式反馈。

- 先核对学段、学科、教材版本、课程标准和既有教学资料，防止版本错配。
- 把学习目标、活动、练习、评价和作业建立可追踪对应关系。
- 区分知识、能力、过程方法和素养目标，并按认知层级与难度检查覆盖。
- 对题目、答案、评分标准和教学结论标注来源及人工复核要求。

## 运行边界

- 本地模型行为：NOT_RUNTIME_VERIFIED
- WorkBuddy平台验证：WORKBUDDY_VALIDATION_NOT_IN_SCOPE
- 本轮不执行上传、安装、审核或正式发布。
