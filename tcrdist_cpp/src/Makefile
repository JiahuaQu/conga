# the compiler
CC = g++

## compiler flags:

# debugging
#CCFLAGS  = -g -std=c++11 -Wall

# production
CCFLAGS  = -O3 -std=c++11 -Wall

# 
INCLUDES = -I ../include/

# recompile if any .hh files changed
HHS = *.hh

all: ../bin/find_neighbors ../bin/calc_distributions ../bin/count_matches_single_chain ../bin/count_matches_paired ../bin/find_paired_matches ../bin/compute_single_chain_distance_matrix


../bin/find_neighbors:  find_neighbors.cc  $(HHS)
	$(CC) $(CCFLAGS) $(INCLUDES) -o ../bin/find_neighbors find_neighbors.cc

../bin/calc_distributions:  calc_distributions.cc  $(HHS)
	$(CC) $(CCFLAGS) $(INCLUDES) -o ../bin/calc_distributions calc_distributions.cc

../bin/count_matches_single_chain:  count_matches_single_chain.cc  $(HHS)
	$(CC) $(CCFLAGS) $(INCLUDES) -o ../bin/count_matches_single_chain count_matches_single_chain.cc

../bin/count_matches_paired:  count_matches_paired.cc  $(HHS)
	$(CC) $(CCFLAGS) $(INCLUDES) -o ../bin/count_matches_paired count_matches_paired.cc

../bin/find_paired_matches:  find_paired_matches.cc  $(HHS)
	$(CC) $(CCFLAGS) $(INCLUDES) -o ../bin/find_paired_matches find_paired_matches.cc

../bin/compute_single_chain_distance_matrix:  compute_single_chain_distance_matrix.cc  $(HHS)
	$(CC) $(CCFLAGS) $(INCLUDES) -o ../bin/compute_single_chain_distance_matrix  compute_single_chain_distance_matrix.cc


clean:
	-rm ./bin/*
