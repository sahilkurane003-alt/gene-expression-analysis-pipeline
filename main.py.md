from Bio import SeqIO



for record in SeqIO.parse("sample.fasta", "fasta"):

&#x20;   seq = record.seq



&#x20;   gc = ((seq.count("G") + seq.count("C")) / len(seq)) \* 100



&#x20;   print("=" \* 40)

&#x20;   print("Sequence ID:", record.id)

&#x20;   print("DNA Sequence:", seq)

&#x20;   print("Length:", len(seq))

&#x20;   print("GC Content:", round(gc, 2), "%")

&#x20;   print("Reverse Complement:", seq.reverse\_complement())

# &#x20;   

