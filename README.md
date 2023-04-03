# CarryLookAheadAdder_4bit

How	does	a	Carry	Look-ahead	Adder	work?	

• The	propagation	delay	of	an	n-bit	ripple	carry	order	is	
proportional	to	n.	
 Due	to	the	rippling	effect	of	carry	sequentially	from	one	stage	to	the	next.	
 
• One	possible	way	to	speedup	the	addition.	

– Generate	the	carry	signals	for	the	various	stages	in	parallel.

Consider	the	i-th	stage	in	the	addition	process.

• We	define	the	carry	generate	and	carry	propagate	
functions	as:

gi	=	Ai.Bi

pi	=	Ai ⊕	Bi	

output	carry ci+1=	gi+pi.ci


	
