# Probabilistic Sponge
challenge.py是一份缩减版 sponge 实现，不是标准SHA-3。题目输入为48-bit seed，输出为digest。

远程服务支持以下命令:

digest <seed>
trace <mode> <seed>
submit <seed_a> <seed_b> <proof>

题目目标是提交一组满足服务端校验条件的种子对。proof 依赖当前连接下发的 nonce，不能直接复用旧连接的数据。
建议先阅读challenge.py和论文，再根据远程接口组织自己的分析与搜索流程。
