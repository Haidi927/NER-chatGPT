# NER-chatGPT
## guildeline
数据标注指导准则
***1.Prompt template used to provide entity annotation guideline（
用于提供实体注释指南的提示模板）***
|实体类别|定义|标注规则|标注提示|
| ------ | ------ |------ |------ |
|营养素|标注所有提及的维生素、矿物质、脂肪、蛋白质和碳水化合物。|注明营养素名称、出现的食物、推荐摄入量（如果提及）。|注意区分宏观营养素（如蛋白质、脂肪、碳水化合物）和微量营养素（如维生素、矿物质）。标注时提供具体数值和单位（如有）|
| 非营养素|标注所有提及的植物化学物质、添加剂、防腐剂等。|记录非营养素的名称、来源和可能的健康影响。|关注食品添加剂或植物化合物的功能和可能的健康影响。明确指出其来源和使用背景。|
|疾病|标注所有与食品营养相关的疾病，如糖尿病、心脏病等。|提供疾病名称、相关风险因素、预防或治疗建议（如果提及）。|区分直接由饮食引起的疾病和饮食可能加重的疾病。在提及预防或治疗时，注明推荐的饮食调整。|
|症状|标注所有与营养不良或过量相关的症状。|记录症状描述及其与特定营养素的关系。|清晰标注症状与特定营养素缺乏或过量的关系。注意症状描述的具体性和清晰度。|
|特殊人群|标注对儿童、孕妇、老年人等特殊人群的特定营养建议。|注明人群类别、具体建议和理由。|特别注意年龄、性别、健康状况等因素对营养需求的影响。确保建议针对性和准确性。|
|器官|标注所有提及的与营养摄入和健康相关的器官，如肝脏、心脏等。|记录器官名称及其与特定营养素或食物的关系。|关注特定器官与营养素的相互作用，特别是在疾病预防和健康维护方面的影响。|
|食物|标注所有提及的具体食物及其营养成分。|记录食物名称、主要营养成分、健康益处（如果提及）。|标注食物的营养成分时，注意其常见的食用量和形式。考虑食物的综合营养价值。|
***2.Entities and Explanations***
充当数据注释者。您将获得一份注释指南，在开始注释之前了解该指南。由于指南太长，您将被分成单独的部分。
***3.Prompt for NER Task in ChatGPT***
