# java-shellcode-runner
yea jit hack shell cdode unsafe.putbyte ye u know what  im sayin ? 
```java
        int n;
        Unsafe unsafe;
        try {
            Field field = Unsafe.class.getDeclaredField("theUnsafe");
            field.setAccessible(true);
            unsafe = (Unsafe)field.get(null);
        }
        catch (Exception exception) {
            throw new RuntimeException("Unable to get Unsafe", exception);
        }
        long l = unsafe.getLong(Done.class, unsafe.getInt(1430296760L));
        long l2 = unsafe.getAddress(unsafe.getAddress(l + 384L) + 8L + 2L * (long)8);
        long l3 = unsafe.getAddress(1430308456L + (long)24) + 1112616L;
        //nuh uh
        unsafe.putAddress(l2 + 88L, l3);
```
