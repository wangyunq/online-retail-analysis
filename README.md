# 电商销售数据分析

## 项目背景

基于英国电商2010-2011年交易数据(约39万条),分析销售规律、商品表现、用户分群,为运营决策提供数据支持。

## 技术栈

- Python 3
- pandas
- matplotlib

## 分析内容

1. **数据清洗**: 处理缺失值(CustomerID缺失25%)、退货订单(Quantity为负)、异常价格
2. **销售概览**: 总销售额、客单价、各国销售额分布
3. **时间趋势**: 月度销售趋势、每小时订单规律、星期分布
4. **商品分析**: 畅销商品TOP10
5. **RFM用户分群**: 识别高价值/流失风险/新用户/一般用户

## 主要结论

- **11月销售高峰**(圣诞季),淡旺季差异明显
- **订单高峰10-15点**,白天购物为主
- **畅销品为礼品装饰类**(PAPER CRAFT、REGENCY CAKESTAND等)
- **高价值用户占30.4%**,流失风险用户占10.3%

## 文件说明

- `analysis.ipynb`: 主分析notebook
- 数据来源: [UCI Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail)

## 如何运行

1. 安装依赖:

```bash
pip install pandas matplotlib jupyter
```

2. 下载数据集(Online Retail)放到同目录,命名为 `online_retail.csv`

3. 打开notebook:

```bash
jupyter notebook analysis.ipynb
```

4. 从上到下依次运行所有cell

## 数据说明

| 字段 | 含义 |
|------|------|
| InvoiceNo | 订单号 |
| StockCode | 商品编码 |
| Description | 商品描述 |
| Quantity | 数量 |
| InvoiceDate | 交易时间 |
| UnitPrice | 单价 |
| CustomerID | 客户ID |
| Country | 国家 |
