``w.online_tables``: Online Tables
==================================
.. currentmodule:: databricks.sdk.service.catalog

.. py:class:: OnlineTablesAPI

    Online tables provide lower latency and higher QPS access to data from Delta tables.

    .. py:method:: create(table: OnlineTable) -> Wait[OnlineTable]

        Create a new Online Table.

        :param table: :class:`OnlineTable`
          Specification of the online table to be created.

        :returns:
          Long-running operation waiter for :class:`OnlineTable`.
          See :method:wait_get_online_table_active for more details.
        

    .. py:method:: create_and_wait(table: OnlineTable, timeout: datetime.timedelta = 0:20:00) -> OnlineTable


    .. py:method:: delete(name: str)

        Delete an online table. Warning: This will delete all the data in the online table. If the source
        Delta table was deleted or modified since this Online Table was created, this will lose the data
        forever!

        :param name: str
          Full three-part (catalog, schema, table) name of the table.


        

    .. py:method:: get(name: str) -> OnlineTable

        Get information about an existing online table and its status.

        :param name: str
          Full three-part (catalog, schema, table) name of the table.

        :returns: :class:`OnlineTable`
        

    .. py:method:: wait_get_online_table_active(name: str, timeout: datetime.timedelta = 0:20:00, callback: Optional[Callable[[OnlineTable], None]]) -> OnlineTable
