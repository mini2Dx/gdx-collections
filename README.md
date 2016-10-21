# gdx-collections
LibGDX collection classes extracted into a standalone library (i.e. no OpenGL, LWJGL, etc. required)

## Mechanism

The gradle build will checkout a specific version of libgdx, copy the collections source files into src/main/java and compile the standalone jar. However MathUtils, RandomXS128 and com.badlogic.gdx.util.reflect classes are required for the collection classes. To allow the collection classes to remain standalone, these classes are copied into _com.badlogic.gdx.utils.compat_ and the references are updated in the collections classes.

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