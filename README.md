# Modeling

  本研究针对商品期货短期价格波动预测的复杂性问题，构建了一种融合时序分解与
深度学习的混合预测模型，旨在提升高频交易场景下的预测精度与稳健性。基于 2017 年
至 2025 年七类主力合约的 1 分钟级数据，通过 ARIMA 剥离线性趋势成分，结合 CNN-
LSTM 网络捕捉局部价格形态与跨周期依赖关系，并引入注意力机制强化关键时段信号
提取，最终采用 XGBoost 集成多源特征实现非线性建模。模型创新性设计了动态量价特
征体系，包括持仓量变动率与价量滚动相关系数，有效量化市场情绪与资金流向的交互
效应。灵分析了卷积核数量与树深度的最优参数区间，同时发现 RSI 与持仓量变动率为
核心预测因子。研究进一步指出模型对外部事件响应滞后与计算效率的局限性，提出引
入实时新闻情感分析模块与模型轻量化压缩的改进路径。本成果不仅为商品期货量化交
易提供了可靠工具，其模块化架构可扩展至股指期货、期权波动率预测等领域，并为电
力、交通等复杂时序预测问题提供方法论借鉴，具备跨学科推广价值。


完整目录结构如下

## C422

> decrease
>
> > HC.csv
> >
> > I.csv
> >
> > JM.csv
> >
> > RB.csv
> >
> > SF.csv
> >
> > SM.csv
> >
> > SS.csv
>
> net
>
> > model
> >
> > >  cnn_lstm_model(1).h5
> > >
> > >  cnn_lstm_mnodel.keras
> > >
> > >  fixed_cnn_lstm_model2.h5
> > >
> > >  fixed_cnn_lstm_model2.keras
> > >
> > >  fixed_cnn_lstm_model3.h5
> > >
> > >  fixed_cnn_lstm_model3.keras
> > >
> > >  xgb_model.jason
> > >
> > >  xgb_model2.jason
> > >
> > >  xgb_model.onnx
> >
> > scalers
> >
> > > scaler_vol.pkl
> > >
> > > scaler_price.pkl
> >
> > arima.ipynb
> >
> > chao.ipynb
> >
> > final.ipynb
> >
> > MA.ipynb
> >
> > erged_data2.csv
> >
> > model.ipynb
> >
> > newsolution.ipynb
> >
> > Papers.docx
> >
> > test.ipynb
> >
> > Untitled.ipynb
>
> c题.pdf
>
> draw.ipynb
>
> feature_ablation.png
>
> merge.csv
>
> normalized_vol.csv
>
> test.ipynb
>
> xgboost_heatmap.png
>
> zip.ipynb
>
> 分步解决方案.md
>
> 分步解决方案：模型预测与结果获取.md
>
> 灵敏度分析.md
>
> 商品期货数据预处理与特征提取完整流程.md
>
> wdaaw
