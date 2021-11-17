# jmeter-protobuf-test
1. 根据protobuf生成java类
2. 配置protoUrlMap.properties,key=请求path value=请求和响应的protobuf类，如果没有空然后,隔开
3. 打开jmeter，创建thread group->sampler->java request
4. 选择com.protobuftest.ProtobufRestfulSample
5. 配置参数，protobuf类里面的参数设置proto.属性名

注意目前不支持枚举参数