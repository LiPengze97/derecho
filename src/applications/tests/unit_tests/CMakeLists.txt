cmake_minimum_required(VERSION 2.8)
set(CMAKE_DISABLE_SOURCE_CHANGES ON)
set(CMAKE_DISABLE_IN_SOURCE_BUILD ON)

include_directories(${CMAKE_SOURCE_DIR}/include)
include_directories(${CMAKE_CURRENT_SOURCE_DIR})

add_executable(rpc_function_types rpc_function_types.cpp)
target_link_libraries(rpc_function_types derecho)

add_executable(rpc_reply_maps rpc_reply_maps.cpp)
target_link_libraries(rpc_reply_maps derecho)

# cooked_send_test
add_executable(cooked_send_test cooked_send_test.cpp)
target_link_libraries(cooked_send_test derecho)

# delivery_order_test
add_executable(delivery_order_test delivery_order_test.cpp)
target_link_libraries(delivery_order_test derecho)

add_executable(subgroup_function_tester subgroup_function_tester.cpp)
target_link_libraries(subgroup_function_tester derecho)

add_executable(log_restart_test log_restart_test.cpp)
target_link_libraries(log_restart_test derecho)

add_executable(signed_log_test signed_log_test.cpp)
target_link_libraries(signed_log_test derecho)

add_executable(openssl_test openssl_test.cpp)
target_link_libraries(openssl_test derecho)

add_executable(signature_chain_test signature_chain_test.cpp)
target_link_libraries(signature_chain_test derecho)