# qualification
近两年我组织的实战训练营/开发认证我自己都没有实际写过，想着有技术教练撑场面，我又何必献丑，我只是早通过几年而已。但作为评委，长时间不现场参加编码，渐渐有些讲不出什么东西，导致训练营的效果相比去年有些打折扣了。近期准备挑个题目练个手，感兴趣的读者可以跟着练。题目是集中6-7个小时可以写完的，但业余很难有这么大块的时间，我准备按迭代拆分，每周发布一个迭代，总共3个迭代。

过程中我会把我的思路附上，顺便讲一些东西提醒注意。参加过一次训练营的人，配合一些知识点的自学，第二次有很大概率能通过认证。训练过程中需要注意的内容不一定很高端（可能不会用到多厉害的算法），但一定是程序员从初级到中级的必备素质。所以忌抬杠，宜分享不同思路。最后我会发布一下评分标准。

这类题目开放性比较大，不定函数，不定入参，不定用例，模拟真实需求开发的过程，跟着来一次就会了。

题目背景：

一副扑克牌（Poker）由52张正牌和2张鬼牌（大王、小王）组成，52张牌分为四组，分别为红桃（Hearts）、黑桃（Spaders）、方块（Diamonds）、梅花（Clubs），每组由A,2,3,4,5,6,7,8,9,10,J,Q,K 13张牌组成。



要求：

使用成熟测试框架（不会搭测试框架的，请回看我ubuntu+vscode+gtest的相关文章）
使用C语言（其他语言也可以，但其他语言我只是初学者，不同语言之间不具有可比性。后面我可能会找一份python的编码结果学习一下）
按照TDD要求编码（不了解TDD的，请回看我之前的文章）
按照简单设计四原则进行编码（不了解TDD的，请回看我之前的文章）
满足编码规范，考虑正交原则、SOLID原则等（编码规范我没写过相关文章，本次穿插一下，设计原则请回看我之前的文章）
如果可能，请考虑性能（性能考虑点，请回看我之前的文章）


迭代一

抽出大王、小王后，在剩余52张牌中抽一张牌比大小，规则如下：

点数大小：A>K>Q>J>10>9>8>7>6>5>4>3>2

花色大小：黑桃>红桃>梅花>方块
