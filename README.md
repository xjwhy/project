# project
Carla simulator with RL
该分支主要是用于跑baseline，和它做一个比较，参数如下所示：
            "args":[
                "--root_dir", "logs/demo/",
                "--experiment_name", "latent_sac",
                "--gin_file", "params.gin",
                "--gin_param", "load_carla_env.port=2000"
            ],
            "env": {
                "CUDA_VISIBLE_DEVICES":"0",
                "PYTHONPATH":"${workspaceRoot}"
            }
