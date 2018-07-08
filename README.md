## 项目: 为CharityML寻找捐献者

### 项目说明
CharityML 是一个位于硅谷中心的虚拟慈善机构，该机构的使命是向渴望学习机器学习技术的人士提供资金支持。在向社区发送接近 32,000 封信件后， CharityML 发现他们收到的捐款都来自年收入超过 50,000 美元的人群。为了扩大潜在捐助者群体，CharityML 决定向加利福尼亚州居民发送信件，但是仅向很可能会给机构捐款的人士发信。加利福尼亚州有接近 1500 万劳动人口，CharityML 请你加入他们的团队，帮助他们构建一个能够准确发现潜在捐助者并降低邮件发送成本的算法。你的目标是评估并优化多个不同的监督学习器，判断哪个算法将能够带来最高的捐款，同时减少发送的信件总数。

### 数据

修改的人口普查数据集含有将近32,000个数据点，每一个数据点含有13个特征。这个数据集是Ron Kohavi的论文*"Scaling Up the Accuracy of Naive-Bayes Classifiers: a Decision-Tree Hybrid",*中数据集的一个修改版本。你能够在[这里](https://www.aaai.org/Papers/KDD/1996/KDD96-033.pdf)找到论文，在[UCI的网站](https://archive.ics.uci.edu/ml/datasets/Census+Income)找到原始数据集。

**特征**

- `age`: 一个整数，表示被调查者的年龄。 
- `workclass`: 一个类别变量表示被调查者的通常劳动类型，允许的值有 {Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked}
- `education_level`: 一个类别变量表示教育程度，允许的值有 {Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool}
- `education-num`: 一个整数表示在学校学习了多少年 
- `marital-status`: 一个类别变量，允许的值有 {Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse} 
- `occupation`: 一个类别变量表示一般的职业领域，允许的值有 {Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces}
- `relationship`: 一个类别变量表示家庭情况，允许的值有 {Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried}
- `race`: 一个类别变量表示人种，允许的值有 {White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black} 
- `sex`: 一个类别变量表示性别，允许的值有 {Female, Male} 
- `capital-gain`: 连续值。 
- `capital-loss`: 连续值。 
- `hours-per-week`: 连续值。 
- `native-country`: 一个类别变量表示原始的国家，允许的值有 {United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands}

**目标变量**

- `income`: 一个类别变量，表示收入属于那个类别，允许的值有 {<=50K, >50K}


### 项目文件
此项目包含三个文件：

- finding_donors.ipynb：主文件。
- census.csv：项目数据集。你将在 notebook 中加载此数据。
- visuals.py：此 Python 脚本提供了项目的补充可视化内容。
