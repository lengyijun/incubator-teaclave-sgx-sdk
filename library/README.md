alloc(origin)
core(origin)
panic_abort(sgx_panic_abort)
panic_unwind(sgx_panic_unwind)
proc_macro(dummy)
rustc-std-workspace-alloc(origin)
rustc-std-workspace-core(origin)
rustc-std-workspace-std(origin)
sgx_alloc
sgx_backtrace
sgx_backtrace_sys
sgx_build_helper
sgx_demangle
sgx_libc
sgx_tprotected_fs
sgx_trts
sgx_types
sgx_unwind
std(sgx_tstd)
stdarch(origin)
term(origin)
test(origin)

# known problems
- trts has to be compiled twice if imported in your enclave code
- features of std

# TODO
- maybe core,alloc... can use a soft link?
- sgx__rand need to be fixed
