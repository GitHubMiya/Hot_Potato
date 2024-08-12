# Hot_Potato
Our game simulates a breadboard version of Hot Potato, where players use personal buttons to control their roles. The "Hot Potato" is represented by LED lights passed between buttons. Players track progress via flashing LEDs and vibrations. As players are eliminated, the game speed increases. An FPGA connects the LEDs and buttons.
module timer (
    input reg [7:0] count,
    input reg clk,
    input reset,

    output elimination,
);
    
//Timer automatically starts when power is supplied




//When reset is 1 counter is reset on every clock pusle counter counts up
always @(posedge clk or negedge reset) begin
    if (~reset) begin
        count <= 0; // Reset counter to 0
    end else if (start) begin
        count <= count + 1; // Increment counter
    end
end


//counter sends signal to Eliminiation and resets when it hits 30
    if count = 30
    elimination <= 1
    reset = 0

    if count = 20
    elimination <= 1
    reset = 0

    if count 
    elimination <= 1
    reset = 0
    

)
