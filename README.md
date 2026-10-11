# 电商销售数据分析 
## 项目背景 基于英国电商2010-2011年交易数据(约39万条),分析销售规律、商品表现、用户分群,为运营决策提供数据支持。 
## 技术栈 
Python, pandas, matplotlib 
## 分析内容 
1. 数据清洗:处理缺失值、退货订单、异常价格
2. 销售概览:各国销售额分布
3. 时间趋势:月度趋势、时段规律、星期规律
4. 商品分析:畅销商品TOP10
5. RFM用户分群:识别高价值/流失风险/新用户/一般用户 
## 主要结论 
- 11月销售高峰(圣诞季),淡旺季差异大
- - 订单高峰10-15点,白天购物为主
  - - 畅销品为礼品装饰类
    - - 高价值用户占30%,流失风险用户占10% 
## 文件说明 
- `analysis.ipynb` : 主分析notebook
- - 数据来源: UCI Online Retail Dataset
## 如何运行
1. 安装依赖: `pip install pandas matplotlib jupyter`
2. 下载数据集放到同目录
3. 打开notebook: `jupyter notebook analysis.ipynb`
