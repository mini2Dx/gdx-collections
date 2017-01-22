# gdx-collections
LibGDX collection classes extracted into a standalone library (i.e. no OpenGL, LWJGL, etc. required)

## Mechanism

The gradle build will checkout a specific version of libgdx, copy the collections source files into src/main/java, rename the packages from _com.badlogic_ to _org.mini2Dx_ and compile the standalone jar.

However MathUtils, RandomXS128 and com.badlogic.gdx.util.reflect classes are required for the collection classes. To allow the collection classes to remain standalone, these classes are copied into _org.mini2Dx.gdx.utils.compat_ and the references are updated in the collections classes.

## Usage

```gradle
compile "org.mini2Dx:gdx-collections:1.9.5"
```

## Included Classes

 * Array
 * ArrayMap
 * AtomicQueue
 * Bits
 * BooleanArray
 * ByteArray
 * CharArray
 * ComparableTimSort
 * DelayedRemovalArray
 * Disposable
 * FloatArray
 * FlushablePool
 * GdxRuntimeException
 * IdentityMap
 * IntArray
 * IntFloatMap
 * IntIntMap
 * IntMap
 * IntSet
 * LongArray
 * LongMap
 * NumberUtils
 * ObjectFloatMap
 * ObjectIntMap
 * ObjectMap
 * ObjectSet
 * OrderedMap
 * OrderedSet
 * Pool
 * PooledLinkedList
 * Pools
 * Predicate
 * Queue
 * QuickSelect
 * ReflectionPool
 * Select
 * ShortArray
 * SnapshotArray
 * Sort
 * SortedIntList
 * TimSort
 * TimeUtils