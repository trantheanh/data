contain **text** -> branch_1 = text_net(feature)
<br />
contain **creative** -> branch_2 = attention_net([creative_net(feature) for feature in features])
<br />
contain **cmeta** -> branch_3 = cmeta_net(feature)
<br />
contain **qmeta** -> branch_4 = qmeta_net(feature)
<br />
output = attention_net([branch_1, branch_2, branch_3, branch_4])

