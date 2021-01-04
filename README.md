gdx-collections
======================
[LibGDX](https://libgdx.badlogicgames.com/) [collection classes](https://github.com/libgdx/libgdx/wiki/Collections) extracted into a standalone library (i.e. no OpenGL, LWJGL, etc. required)

This is useful for those who need high performance collections on the JVM but aren't building an application with LibGDX.

Mechanism
----------------------

The gradle build will checkout a specific version of libgdx, copy the collections source files into src/main/java, rename the packages from _com.badlogic_ to _org.mini2Dx_ and compile the standalone jar.

However MathUtils, RandomXS128 and com.badlogic.gdx.util.reflect classes are required for the collection classes. To allow the collection classes to remain standalone, these classes are copied into _org.mini2Dx.gdx.utils.compat_ and the references are updated in the collections classes.

Usage
----------------------

```gradle
compile "org.mini2Dx:gdx-collections:1.9.12"
```

Included Classes
----------------------

 * [Array](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/Array.html)
 * [ArrayMap](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/ArrayMap.html)
 * [AtomicQueue](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/AtomicQueue.html)
 * [Bits](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/Bits.html)
 * [BooleanArray](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/BooleanArray.html)
 * [ByteArray](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/ByteArray.html)
 * [CharArray](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/CharArray.html)
 * [DelayedRemovalArray](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/DelayedRemovalArray.html)
 * [Disposable](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/Disposable.html)
 * [FloatArray](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/FloatArray.html)
 * [FlushablePool](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/FlushablePool.html)
 * [GdxRuntimeException](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/GdxRuntimeException.html)
 * [IdentityMap](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/IdentityMap.html)
 * [IntArray](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/IntArray.html)
 * [IntFloatMap](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/IntFloatMap.html)
 * [IntIntMap](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/IntIntMap.html)
 * [IntMap](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/IntMap.html)
 * [IntSet](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/IntSet.html)
 * [LongArray](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/LongArray.html)
 * [LongMap](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/LongMap.html)
 * [NumberUtils](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/NumberUtils.html)
 * [ObjectFloatMap](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/ObjectFloatMap.html)
 * [ObjectIntMap](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/ObjectIntMap.html)
 * [ObjectMap](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/ObjectMap.html)
 * [ObjectSet](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/ObjectSet.html)
 * [OrderedMap](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/OrderedMap.html)
 * [OrderedSet](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/OrderedSet.html)
 * [Pool](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/Pool.html)
 * [PooledLinkedList](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/PooledLinkedList.html)
 * [Pools](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/Pools.html)
 * [Predicate](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/Predicate.html)
 * [Queue](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/Queue.html)
 * [QuickSelect](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/QuickSelect.html)
 * [ReflectionPool](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/ReflectionPool.html)
 * [Select](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/Select.html)
 * [ShortArray](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/ShortArray.html)
 * [SnapshotArray](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/SnapshotArray.html)
 * [Sort](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/Sort.html)
 * [SortedIntList](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/SortedIntList.html)
 * [TimeUtils](https://libgdx.badlogicgames.com/ci/nightlies/docs/api/com/badlogic/gdx/utils/TimeUtils.html)
