# O2O优惠券预测项目
一、项目简介
本项目为天池中的练习赛，数据集源自2016年上半年（即1-6月份）真实的线上线下消费行为，我们需要根据用户在2016年1月1日至2016年6月30日之间真实线上线下消费行为，预测用户在2016年7月份领取优惠券后的15天内使用和消费情况
二、项目目标
预测投放的优惠券是否核销，通过分析建模，精准预测用户是否会在规定时间内使用相应优惠券
三、评定标准
AUC（Area Under Curve）：ROC曲线与x坐标围成的面积。
ROC曲线：受试者工作特征曲线，ROC曲线是将每个分类模型及其阈值最终的伪阳性率和真阳性率（相当于计算每个雷达兵预报的准确性）体现在，以伪阳性率（FPR）为x轴，真阳性率(TPR)为y轴的二维坐标中，形成的曲线。越靠近左上角的点准确率越高
AUC取在[0，1]，值越大的分类器，正确率越高
四、数据描述
Table 1: 用户线下消费和优惠券领取行为，ccf_offline_stage1_train.csv

Table 2: 用户线上点击/消费和优惠券领取行为，ccf_online_stage1_train

Table 3：用户O2O线下优惠券使用预测样本，ccf_offline_stage1_test_revised.csv

Table 4：选手提交文件字段，其中user_id,coupon_id和date_received均来自Table 3,而Probability为预测值
