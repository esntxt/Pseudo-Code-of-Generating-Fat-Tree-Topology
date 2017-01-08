# Pseudo-Code-of-Generating-Fat-Tree-Topology
1:      class fat-tree topology
2:      {
3:        function addcore switch (){
4:         for i (0→(K/2)2 begin append core switch end for
5:        }
6:        function add aggregation switch and edge switch () {
7:          for i (0→ K2/2) begin append aggregation switch and edge switch end for
8:        }
9:        Function add host (){
10:         for i (0→ K3/4) begin append host end for
11:       }
12:      function add links (){
13:        for i (0→ K2/2) begin
14:         for j (0→ K/2) begin
15:          add link between (edge switch [i], host [j+ K/2*i], j)
16:          end for
17:        for i (0→k) begin
18:         for j (0→ K/2) begin
19:          for z (0→ K/2) begin
20:           add link between
              (aggregation switch[z+ K/2*i], edge switch [z+ K/2*i], z, j+ K/2)
21:           add link between
              (core switch[z+ K/2*j], aggregation switch [i+ K/2*j], I, z+ K/2)
22:          end for
23:        end for
24:       end for
25:      }
26:     }
