# Integrated-Deep-Multiscale-Feature-Fusion-Network
# The dataset can be download in the following website
# "A. Saxena and K. Goebel, Turbofan Engine Degradation Simulation Data Set, NASA Ames Prognostics Data Repository
# (http://ti.arc.nasa.gov/project/prognostic-data-repository), NASA Ames Research Center, Moffett Field, CA, 2008."
# ********************Some pre-processing should be done first*******************,
# ******************including sensor selecting, data min-max scaling (-1,1),
# and 2-D samples design, samples' dimension = (Cycle_number, Sensor_number)*******************

# This part gives an example for samples loading and design
# before load into this code, you can use MATLAB to pre-process the raw data according to the steps above.
# Also you can directly pre-process the raw data using python.
# Moreover, you can replac this part with your own codes programmed according to your own style
# In a word, the final goals are to obtains input data and its labels, their dimensions must be as follows.
# X_train = (Train_sample_number, Cycle_number, Sensor_number, channel_number = 1)
# y_train = (Train_sample_number, 1)
# X_test = (Test_sample_number, Cycle_number, Sensor_number, channel_number = 1)
# y_test = (Test_sample_number, 1)
# Take FD001 for instance, 14 sensors are selected, and each sample contains 30-cycle multi-sensor data,
# that is Cycle_number=30, Sensor_number = 14.
