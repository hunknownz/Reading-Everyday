比特币的网络所有节点都是平等的，加入网络至少有一个种子节点，和种子节点联系，会告诉你它所知道的其他网络节点。节点之间通过tcp通信，这样有利于穿过防火墙。离开不用告诉其他节点，直接关闭应用程序就可以了。别的节点没有听到你的消息，过一段时间就会把你删掉。

比特币网络设定原则是简单鲁棒，非高效。每个节点维护邻区节点集合，消息传播通过flooding的方式，节点第一次听到某个消息，将它传播给其他所有邻居节点 并记录下这个消息我已收到，下次再收到就不会再转发给邻居节点了。
