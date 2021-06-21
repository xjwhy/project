# project
这一版本主要是新环境的baseline：
1、新环境是有3种输入，分别是地图、鸟瞰图、RGB，且环境的状态图像是多帧打包到一起的
2、将evaluate的策略改为贪心的
3、由于环境的变化，将网络结构的代码进行改正,目前是个半成品，是由于修改环境的话，需要改动的太多
4、环境一致设定为动作重复为4，episode最长为256，这样一个episode的batch最大为64,replay_buffer_capacity是1e5，
If out of system memory, change the parameter replay_buffer_capacity and initial_collect_steps the function tran_eval smaller.

If out of CUDA memory, set parameter model_batch_size or sequence_length of the function tran_eval smaller.

