# project
这一版本主要是新环境的baseline，新环境是有3种输入，分别是地图、鸟瞰图、RGB

If out of system memory, change the parameter replay_buffer_capacity and initial_collect_steps the function tran_eval smaller.

If out of CUDA memory, set parameter model_batch_size or sequence_length of the function tran_eval smaller.

