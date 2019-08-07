# event_recommendation
我们有下面这样几类数据 
①：用户的历史数据 => 对 event 是否感兴趣/是否参加 
②：用户社交数据 => 朋友圈 
③：event 相关的数据 => event

简单思考 
①：要把更多维度的信息纳入考量。 
②：协同过滤是基于user -event 历史交互数据。 
③：需要把社交数据和event 相关信息 作为影响最后结果的因素纳入考量。 
④：视作分类模型，每一个人感兴趣/不感兴趣 是 target，其他影响结果的是feature。 
⑤：影响结果的 feature 包括由协同过滤产出的推荐度。（userCF，itemCF）
基于以上的考虑，我们选取几种特征为用户做推荐系统