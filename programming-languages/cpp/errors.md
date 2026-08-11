# C++ Error Codes

This list is heavily based on

* https://en.cppreference.com/w/cpp/error/errc
* https://en.cppreference.com/w/cpp/header/cerrno

**Standard C++ Exceptions**

    std::exception       Base class for all standard exceptions
    std::logic_error     Exception for detectable logic errors
    std::runtime_error   Exception for unexpected runtime errors
    std::out_of_range    Exception thrown when a value is out of range
    std::invalid_argument Exception thrown when an invalid argument is passed
    std::bad_alloc       Exception thrown when memory allocation fails
    std::bad_cast        Exception thrown when a dynamic_cast fails
    std::bad_typeid      Exception thrown when a typeid fails

**C++11 `std::errc` Error Codes**

    e2big                Argument list too long
    address_family_not_supported Address family not supported by protocol
    address_in_use       Address already in use
    address_not_available Cannot assign requested address
    already_connected    Transport endpoint is already connected
    bad_address          Bad address
    bad_file_descriptor  Bad file descriptor
    broken_pipe          Broken pipe
    connection_aborted   Connection aborted
    connection_refused   Connection refused
    connection_reset     Connection reset by peer
    cross_device_link    Invalid cross-device link
    destination_address_required Destination address required
    deadlock             Resource deadlock would occur
    directory_not_empty  Directory not empty
    executable_format_error Exec format error
    file_exists          File exists
    file_too_large       File too large
    illegal_seek         Illegal seek
    inappropriate_fallback Protocol wrong type for socket
    interrupt            Interrupted system call
    io_error             I/O error
    is_a_directory       Is a directory
    message_size         Message too long
    network_down         Network is down
    network_reset        Connection aborted
    network_unreachable  Network unreachable
    no_buffer_space      No buffer space available
    no_child_process     No child processes
    no_link              Link has been severed
    no_message_of_desired_type No message of desired type
    no_protocol_option   Protocol not available
    no_space_on_device   No space left on device
    no_stream_resources  Out of streams resources
    no_such_device       No such device
    no_such_file_or_directory No such file or directory
    no_such_process      No such process
    not_a_directory      Not a directory
    not_a_socket         Socket operation on non-socket
    not_connected        Transport endpoint is not connected
    not_enough_memory    Cannot allocate memory
    not_supported        Operation not supported
    operation_canceled   Operation canceled
    operation_in_progress Operation now in progress
    operation_not_permitted Operation not permitted
    operation_now_in_progress Operation already in progress
    operation_would_block Operation would block
    owner_dead           Owner died
    permission_denied    Permission denied
    protocol_error       Protocol error
    protocol_not_supported Protocol not supported
    protocol_wrong_type  Protocol wrong type for socket
    read_only_file_system Read-only file system
    resource_deadlock_would_occur Resource deadlock would occur
    result_too_large     Result too large
    state_not_recoverable State not recoverable
    stream_timeout       Stream timed out
    text_file_busy       Text file busy
    timeout              Connection timed out
    too_many_files_open_in_system Too many open files in system
    too_many_files_open  Too many open files
    too_many_links       Too many links
    too_many_symbolic_link_levels Too many levels of symbolic links
    too_many_users       Too many users
    value_too_large_for_defined_data_type Value too large for defined data type
