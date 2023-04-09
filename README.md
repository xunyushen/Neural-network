# Neural-network

# This constructor expects the user to specify the number of inputs, hidden nodes, hidden layers, and output nodes
__init__(self, num_in_nodes, .....)
                 
# This method is to do the heavy lifting, that is, train neural net, and report error.
# The network configuration should be saved within the network itself at the end of the training. Finally the program will output the correct list of errors based on incremental learning    
train_net_incremental(self, input_list, output_list, max_num_epoch=100000, min_sse=0.001)

#  Feed forward calculate the activation values given the input.
_feed_forward(self, input_list, row)

# These two methods handle the calculations and application of the results of deltas calculations
_calculate_deltas(self, activations, errors, prev_weight_deltas=None)
_adjust_weights_bias(self)
