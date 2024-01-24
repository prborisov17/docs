
# Монтирование бакетов в контейнер

{% include [read-note](../../_includes/functions/read-note.md) %}

Монтирование бакетов позволяет обращаться к бакетам через интерфейс файловой системы. В настройках ревизии контейнера пользователь может указать путь монтирования или несколько. Директория, к которой смонтируется бакет, будет доступна по указанному пути.

Смонтировать можно весь бакет или [папку](../../storage/concepts/object#folder).


{% include [roles-for-bucket-mounting](../../_includes/functions/roles-for-bucket-mounting.md) %}

## См. также {#see-also}

* [Монтировать бакеты в контейнер](../operations/mount-bucket.md)
* [Монтировать бакеты в функцию](../../functions/operations/function/mount-bucket.md)
