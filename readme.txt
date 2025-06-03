rack-labels.txt accompanies the paper "Graph quandles: Generalized Cayley graphs of racks and right quasigroups" by Lực Ta.
It performs an exhaustive search of all vertex markings of a given graph that realize racks and quandles in the sense of Valeriy Bardakov.

To use rack-labels.txt, first load the GRAPE package in GAP:

	LoadPackage("grape");

As an example of how to use rack-labels.txt, here's what you would input to compute the numbers of rack and quandle structures realizable
by cycle graphs C_n of orders 3 to 6; replace "[PATH]" with the path to whereever you've saved rack-labels.txt on your computer:

	labels:= function(m) n:=m; ReadAsFunction(Concatenation([PATH],"rack-labels.txt"))(); end;
	for m in [3..6] do labels(m); od;
