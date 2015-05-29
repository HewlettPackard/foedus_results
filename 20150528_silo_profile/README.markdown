Just for an expected question.

Dragonhawk,
./benchmarks/dbtest --verbose --bench tpcc --num-threads 192 --scale-factor 192 --runtime 30 --numa-memory 384G

perf record -p <pid> --freq=10

Default frequency was too expensive.


    # data0
    25.29%  dbtest  dbtest               [.] Masstree::node_base<masstree_params>::reach_leaf(Masstree::key<unsigned long> const&, basic_nodeversion<nodeversi
    7.69%  dbtest  libc-2.17.so         [.] __memcpy_ssse3_back
    5.23%  dbtest  dbtest               [.] Masstree::unlocked_tcursor<masstree_params>::find_unlocked(simple_threadinfo&)
    4.30%  dbtest  dbtest               [.] transaction<transaction_proto2, hint_tpcc_delivery_traits>::commit(bool)
    3.69%  dbtest  dbtest               [.] bool transaction<transaction_proto2, hint_tpcc_new_order_traits>::do_tuple_read<txn_btree_::single_value_reader>(
    2.73%  dbtest  libstdc++.so.6.0.19  [.] std::string::_M_mutate(unsigned long, unsigned long, unsigned long)
    2.51%  dbtest  dbtest               [.] Masstree::tcursor<masstree_params>::find_locked(simple_threadinfo&)
    2.22%  dbtest  dbtest               [.] rcu::sync::alloc(unsigned long)
    2.19%  dbtest  dbtest               [.] tpcc_worker::txn_new_order()
    1.86%  dbtest  dbtest               [.] transaction<transaction_proto2, hint_tpcc_new_order_traits>::commit(bool)
    1.85%  dbtest  dbtest               [.] str_arena::next()
    1.60%  dbtest  libc-2.17.so         [.] __memset_sse2
    1.60%  dbtest  dbtest               [.] transaction_proto2_static::clean_up_to_including(transaction_proto2_static::threadctx&, unsigned long)
    1.56%  dbtest  [kernel.kallsyms]    [k] native_write_msr_safe
    1.45%  dbtest  [kernel.kallsyms]    [k] update_cfs_rq_blocked_load
    1.38%  dbtest  dbtest               [.] int Masstree::basic_table<masstree_params>::scan<Masstree::forward_scan_helper, mbtree<masstree_params>::low_leve
    1.35%  dbtest  dbtest               [.] bool transaction<transaction_proto2, hint_tpcc_stock_level_read_only_traits>::do_tuple_read<txn_btree_::single_va
    1.35%  dbtest  dbtest               [.] dbtuple::ReadStatus dbtuple::record_at_chain<txn_btree_::single_value_reader, str_arena>(dbtuple const*, unsigned
    1.33%  dbtest  libstdc++.so.6.0.19  [.] std::string::append(unsigned long, char)
    1.24%  dbtest  dbtest               [.] mbtree<masstree_params>::insert_if_absent(varkey const&, unsigned char*, mbtree<masstree_params>::insert_info_t*)
    1.14%  dbtest  dbtest               [.] std::less<transaction_base::dbtuple_write_info>::operator()(transaction_base::dbtuple_write_info const&, transact
    0.80%  dbtest  dbtest               [.] tpcc_worker::txn_payment()
    0.73%  dbtest  dbtest               [.] int Masstree::scanstackelt<masstree_params>::find_next<Masstree::forward_scan_helper>(Masstree::forward_scan_help
    0.70%  dbtest  dbtest               [.] transaction<transaction_proto2, hint_tpcc_payment_traits>::commit(bool)
    0.65%  dbtest  libstdc++.so.6.0.19  [.] std::string::resize(unsigned long, char)
    0.63%  dbtest  [kernel.kallsyms]    [k] smp_call_function_many
    0.60%  dbtest  dbtest               [.] tpcc_worker::txn_delivery()
    0.60%  dbtest  dbtest               [.] allocator::ReleaseArenas(void**)
    0.56%  dbtest  dbtest               [.] Masstree::tcursor<masstree_params>::make_split(simple_threadinfo&)
    0.56%  dbtest  libstdc++.so.6.0.19  [.] std::string::_M_replace_safe(unsigned long, unsigned long, char const*, unsigned long)
    0.55%  dbtest  dbtest               [.] bool transaction<transaction_proto2, hint_tpcc_payment_traits>::do_tuple_read<txn_btree_::value_reader>(dbtuple c
    0.52%  dbtest  dbtest               [.] ndb_ordered_index<transaction_proto2>::get(void*, std::string const&, std::string&, unsigned long)

    # data1
    25.09%  dbtest  dbtest               [.] Masstree::node_base<masstree_params>::reach_leaf(Masstree::key<unsigned long> const&, basic_nodeversion<nodeversio
    8.28%  dbtest  libc-2.17.so         [.] __memcpy_ssse3_back
    5.27%  dbtest  dbtest               [.] Masstree::unlocked_tcursor<masstree_params>::find_unlocked(simple_threadinfo&)
    4.09%  dbtest  dbtest               [.] bool transaction<transaction_proto2, hint_tpcc_new_order_traits>::do_tuple_read<txn_btree_::single_value_reader>(d
    3.34%  dbtest  dbtest               [.] transaction<transaction_proto2, hint_tpcc_delivery_traits>::commit(bool)
    2.83%  dbtest  libstdc++.so.6.0.19  [.] std::string::_M_mutate(unsigned long, unsigned long, unsigned long)
    2.70%  dbtest  dbtest               [.] Masstree::tcursor<masstree_params>::find_locked(simple_threadinfo&)
    2.24%  dbtest  dbtest               [.] rcu::sync::alloc(unsigned long)
    1.89%  dbtest  dbtest               [.] tpcc_worker::txn_new_order()
    1.70%  dbtest  dbtest               [.] bool transaction<transaction_proto2, hint_tpcc_stock_level_read_only_traits>::do_tuple_read<txn_btree_::single_val
    1.70%  dbtest  [kernel.kallsyms]    [k] native_write_msr_safe
    1.70%  dbtest  dbtest               [.] transaction_proto2_static::clean_up_to_including(transaction_proto2_static::threadctx&, unsigned long)
    1.67%  dbtest  dbtest               [.] str_arena::next()
    1.63%  dbtest  dbtest               [.] transaction<transaction_proto2, hint_tpcc_new_order_traits>::commit(bool)
    1.60%  dbtest  dbtest               [.] dbtuple::ReadStatus dbtuple::record_at_chain<txn_btree_::single_value_reader, str_arena>(dbtuple const*, unsigned
    1.52%  dbtest  dbtest               [.] int Masstree::basic_table<masstree_params>::scan<Masstree::forward_scan_helper, mbtree<masstree_params>::low_level
    1.52%  dbtest  dbtest               [.] mbtree<masstree_params>::insert_if_absent(varkey const&, unsigned char*, mbtree<masstree_params>::insert_info_t*)
    1.47%  dbtest  libc-2.17.so         [.] __memset_sse2
    1.45%  dbtest  [kernel.kallsyms]    [k] update_cfs_rq_blocked_load
    1.04%  dbtest  libstdc++.so.6.0.19  [.] std::string::append(unsigned long, char)
    1.01%  dbtest  dbtest               [.] int Masstree::scanstackelt<masstree_params>::find_next<Masstree::forward_scan_helper>(Masstree::forward_scan_helpe
    0.94%  dbtest  dbtest               [.] std::less<transaction_base::dbtuple_write_info>::operator()(transaction_base::dbtuple_write_info const&, transacti
    0.87%  dbtest  dbtest               [.] tpcc_worker::txn_delivery()
    0.80%  dbtest  dbtest               [.] tpcc_worker::txn_payment()
    0.78%  dbtest  [kernel.kallsyms]    [k] smp_call_function_many
    0.77%  dbtest  dbtest               [.] Masstree::tcursor<masstree_params>::make_split(simple_threadinfo&)
    0.68%  dbtest  dbtest               [.] mbtree<masstree_params>::search(varkey const&, unsigned char*&, std::pair<Masstree::leaf<masstree_params> const*,
    0.58%  dbtest  dbtest               [.] transaction<transaction_proto2, hint_tpcc_payment_traits>::commit(bool)
    0.55%  dbtest  libstdc++.so.6.0.19  [.] std::string::resize(unsigned long, char)
    0.54%  dbtest  dbtest               [.] order_line_scan_callback::invoke(char const*, unsigned long, std::string const&)
    0.54%  dbtest  [kernel.kallsyms]    [k] task_tick_fair
    0.50%  dbtest  dbtest               [.] util::fast_random::next_uniform()
    0.50%  dbtest  dbtest               [.] bool transaction<transaction_proto2, hint_tpcc_delivery_traits>::do_tuple_read<txn_btree_::value_reader>(dbtuple c
    0.50%  dbtest  [kernel.kallsyms]    [k] llist_add_batch
    0.48%  dbtest  dbtest               [.] allocator::ReleaseArenas(void**)
    0.48%  dbtest  dbtest               [.] txn_btree_::tuple_writer(dbtuple::TupleWriterMode, void const*, unsigned char*, unsigned long)
    0.45%  dbtest  [kernel.kallsyms]    [k] down_read_trylock
    0.40%  dbtest  libstdc++.so.6.0.19  [.] std::string::_M_replace_safe(unsigned long, unsigned long, char const*, unsigned long)
    0.38%  dbtest  dbtest               [.] static_limit_callback<15ul>::invoke(char const*, unsigned long, std::string const&)

    # data2
    24.33%  dbtest  dbtest               [.] Masstree::node_base<masstree_params>::reach_leaf(Masstree::key<unsigned long> const&, basic_nodeversion<nodeversio
    7.93%  dbtest  libc-2.17.so         [.] __memcpy_ssse3_back
    5.34%  dbtest  dbtest               [.] Masstree::unlocked_tcursor<masstree_params>::find_unlocked(simple_threadinfo&)
    4.03%  dbtest  dbtest               [.] bool transaction<transaction_proto2, hint_tpcc_new_order_traits>::do_tuple_read<txn_btree_::single_value_reader>(d
    3.35%  dbtest  dbtest               [.] transaction<transaction_proto2, hint_tpcc_delivery_traits>::commit(bool)
    2.95%  dbtest  libstdc++.so.6.0.19  [.] std::string::_M_mutate(unsigned long, unsigned long, unsigned long)
    2.51%  dbtest  dbtest               [.] tpcc_worker::txn_new_order()
    2.50%  dbtest  dbtest               [.] rcu::sync::alloc(unsigned long)
    2.21%  dbtest  dbtest               [.] bool transaction<transaction_proto2, hint_tpcc_stock_level_read_only_traits>::do_tuple_read<txn_btree_::single_val
    2.19%  dbtest  dbtest               [.] str_arena::next()
    2.17%  dbtest  dbtest               [.] Masstree::tcursor<masstree_params>::find_locked(simple_threadinfo&)
    2.12%  dbtest  [kernel.kallsyms]    [k] update_cfs_rq_blocked_load
    1.55%  dbtest  dbtest               [.] transaction_proto2_static::clean_up_to_including(transaction_proto2_static::threadctx&, unsigned long)
    1.46%  dbtest  dbtest               [.] dbtuple::ReadStatus dbtuple::record_at_chain<txn_btree_::single_value_reader, str_arena>(dbtuple const*, unsigned
    1.45%  dbtest  [kernel.kallsyms]    [k] native_write_msr_safe
    1.32%  dbtest  dbtest               [.] transaction<transaction_proto2, hint_tpcc_new_order_traits>::commit(bool)
    1.31%  dbtest  dbtest               [.] std::less<transaction_base::dbtuple_write_info>::operator()(transaction_base::dbtuple_write_info const&, transacti
    1.25%  dbtest  libc-2.17.so         [.] __memset_sse2
    1.14%  dbtest  libstdc++.so.6.0.19  [.] std::string::append(unsigned long, char)
    1.11%  dbtest  dbtest               [.] int Masstree::basic_table<masstree_params>::scan<Masstree::forward_scan_helper, mbtree<masstree_params>::low_level
    0.89%  dbtest  dbtest               [.] int Masstree::scanstackelt<masstree_params>::find_next<Masstree::forward_scan_helper>(Masstree::forward_scan_helpe
    0.86%  dbtest  libstdc++.so.6.0.19  [.] std::string::resize(unsigned long, char)
    0.79%  dbtest  [kernel.kallsyms]    [k] task_tick_fair
    0.78%  dbtest  dbtest               [.] tpcc_worker::txn_delivery()
    0.74%  dbtest  dbtest               [.] tpcc_worker::txn_payment()
    0.72%  dbtest  dbtest               [.] mbtree<masstree_params>::insert_if_absent(varkey const&, unsigned char*, mbtree<masstree_params>::insert_info_t*)
    0.69%  dbtest  dbtest               [.] allocator::ReleaseArenas(void**)
    0.66%  dbtest  libstdc++.so.6.0.19  [.] std::string::_M_replace_safe(unsigned long, unsigned long, char const*, unsigned long)
    0.62%  dbtest  dbtest               [.] Masstree::tcursor<masstree_params>::make_split(simple_threadinfo&)
    0.61%  dbtest  [kernel.kallsyms]    [k] smp_call_function_many
    0.58%  dbtest  dbtest               [.] bool transaction<transaction_proto2, hint_tpcc_payment_traits>::do_tuple_read<txn_btree_::value_reader>(dbtuple co
    0.57%  dbtest  dbtest               [.] transaction<transaction_proto2, hint_tpcc_payment_traits>::commit(bool)
    0.57%  dbtest  dbtest               [.] bool transaction<transaction_proto2, hint_tpcc_delivery_traits>::do_tuple_read<txn_btree_::single_value_reader>(db
    0.56%  dbtest  dbtest               [.] txn_btree_::tuple_writer(dbtuple::TupleWriterMode, void const*, unsigned char*, unsigned long)
    0.52%  dbtest  libc-2.17.so         [.] vfprintf
    0.51%  dbtest  dbtest               [.] ndb_ordered_index<transaction_proto2>::get(void*, std::string const&, std::string&, unsigned long)
    0.47%  dbtest  [kernel.kallsyms]    [k] llist_add_batch
    0.45%  dbtest  [kernel.kallsyms]    [k] update_cfs_shares
    0.45%  dbtest  dbtest               [.] order_line_scan_callback::invoke(char const*, unsigned long, std::string const&)
