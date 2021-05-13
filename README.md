# project
Carla simulator with RL
该分支主要是用于跑baseline，和它做一个比较，参数如下所示：
            "args":[
                "--root_dir", "logs/main/",
                "--experiment_name", "latent_sac",
                "--gin_file", "params.gin",
                "--gin_param", "load_carla_env.port=2000"
            ],
            "env": {
                "CUDA_VISIBLE_DEVICES":"0",
                "PYTHONPATH":"${workspaceRoot}"
            }

If out of system memory, change the parameter replay_buffer_capacity and initial_collect_steps the function tran_eval smaller.

If out of CUDA memory, set parameter model_batch_size or sequence_length of the function tran_eval smaller.

