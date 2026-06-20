# 数字逻辑

示例页面。以后可以把坦克对战大程的设计笔记放这里。

## Verilog 代码块

```verilog
module counter (
    input  wire clk,
    input  wire rst_n,
    output reg [3:0] cnt
);
    always @(posedge clk or negedge rst_n) begin
        if (!rst_n) cnt <= 4'd0;
        else        cnt <= cnt + 1'b1;
    end
endmodule
```

!!! warning "Vivado 路径提醒"
    工程路径不要含中文和空格，否则综合/实现可能莫名报错。
