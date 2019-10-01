### ES

`index` `type` `body` `article` `properties` `analyzer` `store`

[elasticsearch](https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-5.6.1.tar.gz) [kibana](https://artifacts.elastic.co/downloads/kibana/kibana-5.6.1-linux-x86_64.tar.gz) [x-pack](https://artifacts.elastic.co/downloads/packs/x-pack/x-pack-5.6.1.zip) [nodejs](https://nodejs.org/dist/v10.16.3/node-v10.16.3.tar.gz) [elasticsearch-head-master](https://github.com/mobz/elasticsearch-head/tree/master) [安装x-pack](https://blog.csdn.net/qqqq0199181/article/details/83017641) [安装head](https://blog.csdn.net/FromTheWind/article/details/91367275) 

#### 近实时

`1s`

#### CLuster

`集群`

#### Node

`节点`

#### Index

`数据库` `Database` `索引`

`article` `comment` 

#### Type

​	`表` `table` `类型`

#### Document

 `行` `数据行` `Row`

#### Field

`列` `字段` `Column`

#### Mapping

`类类型` `是否存储` `是否分词` `约束` `Schema` `映射`

#### Article

`索引区域` `数据区域` 

```javascript
client.indeces.putMapping({
    index:'blog',
    type:'article',
    body:{
        article:{
            properties:{
                id:{
                    type:'string',
                    analizer:'ik',
                    store:'yes'
                },
                title:{
                    type:'string',
                    analizer:'ik',
                    store:'yes'
                },
                content:{
                    type:'string',
                    analizer:'ik',
                    store:'yes'
                }
            }
        }
    }
})
```