2024-10-24记录
1、通过STM32CubeMX生成的第一代工程文档，然后将Main中的注释删除。同时，将优化等级改为0。
2、STM32CubeMX的配置 放在 STM32CubeMX_Config文件夹中
3、将app_freertos.c中的原生注释给删除掉
2024-10-25记录
1、添加EasyLogger日志。注意：Easylogger(ROM<1.6K, RAM<0.3K)
github路径 https://github.com/armink/EasyLogger?tab=readme-ov-file

注意：elog_port_get_t_info、elog_port_get_p_info、elog_port_get_time 被强制写为空
    日志输出接口 elog_port_output 尚未绑定
    且该文件为第一版文件 因此 内部的很多参数 都没有进行调整和优化