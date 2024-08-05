.PHONY: build publish

build:
	rooch move build  --named-addresses task4=default

publish:
	rooch move publish  --named-addresses task4=default

uxto:
	rooch rpc request --method btc_queryUTXOs --params '[{"owner":"tb1p5tznpmyxya5tmvq4ctj084tsffduh6wy0qfj9cy3kkctzechvx5qg6xxtp"}, null, "3", true]'

mint:
	rooch move run --function default::task4::mint --args 'string:test' --args 'object_id:0x826a5e56581ba5ab84c39976f27cf3578cf524308b4ffc123922dfff507e514decd19caae78d9ecf3f85ea71ed0e7528f61a16942b31ab1434efa6011e48ddcf'

# 0x7a21c2243f81236e0296db0f12936c7709fcd75c013580537e429bfe3513f170::task4