module add_full
(
input wire a,
input wire b,
input wire ci,
output wire s,
output wire co
);
assign s = a ^ b ^ ci;
assign co = (a & b) | (b & ci) | (a & ci);
endmodule
