benchmark(name='scala',
  dependencies=[
    pants('3rdparty:caliper'),
    pants('3rdparty:scala-library'),
    pants('util/util-core/src/main/scala'),
    pants('util/util-jvm/src/main/scala')
  ],
  sources=rglobs('*.scala')
)

jvm_binary(name='caliper',
  main='com.google.caliper.Runner',
  dependencies=[
    pants(':scala')
  ]
)
