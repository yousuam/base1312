# base1312
Exporting Blocks to JSON
import json

blocks = []
for i in range(latest-10, latest):
    blocks.append(dict(w3.eth.get_block(i)))

json.dump(blocks, open("blocks.json", "w"))
