class Solution:
    def largestTriangleArea(self, points: List[List[int]]) -> float:
        return max(abs(0.5*(x1*(y2-y3)+x2*(y3-y1)+x3*(y1-y2))) for [x1,y1], [x2,y2], [x3,y3] in combinations(points, 3))




