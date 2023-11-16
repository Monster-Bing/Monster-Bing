这是一个用python语言编写的合并两个有序数组的函数
class Solution(object):
    def merge(self, nums1, m, nums2, n):
        merged = []
        i, j = 0, 0
    
        while i < m and j < n:
            if nums1[i] <nums2[j]:
                merged.append(nums1[i])
                i += 1
            else:
                merged.append(nums2[j])
                j += 1
        while i < m:
            merged.append(nums1[i])
            i += 1
        
        while j < n:
            merged.append(nums2[j])
            j += 1
        nums1[:m+n] = merged
